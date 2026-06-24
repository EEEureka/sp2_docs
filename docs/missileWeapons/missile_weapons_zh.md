# 导弹武器锁定时长

## 1. 锁定时长计算方式

### 1.1 锁定速率 $r$

- 先计算锁定速率 $r$：

```math
r=\max\left(\mathrm{clamp}\left(\frac{\text{signature}}{\text{distance}}\cdot \text{SeekerSensitivity},\,0,\,2\right),\,0.1\right)
```

- 若为连续照射锁，则再乘以 $1.5$：

```math
r \leftarrow 1.5r
```

### 1.2 锁定进度 $L$

- 锁定进度更新为：

```math
L_{t+\Delta t}=\min(1,\,L_t+r\Delta t)
```

  其中 $L$ 表示锁定进度百分比，当 $L=1$ 时即为已锁定状态。
- 取消对目标锁定后，锁定进度会衰减：

```math
L_{t+\Delta t}=\max(0,\,L_t-0.5\Delta t)
```

### 1.3 理论锁定时长（不被干扰）

```math
T_{\text{lock}}=\frac{1}{r}
```

## 2. 关键参数说明

### 2.1 SeekerSensitivity（导引头灵敏度）

- 红外导引头：5
- 雷达导引头：25
- 激光导引头：2500
- 反辐射导引头：5

### 2.2 Signature（目标特征强度）

> 该参数表示导弹导引头接收的目标信号特征强度，受目标类型与导引头类型影响。

#### 2.2.1 Signature 取值矩阵（按目标类型 × 导引头模式）

| 导引头模式 \ 目标类型 | 地面目标 | 激光指示器目标 | 玩家目标 |
|---|---:|---:|---|
| 无导引头 | - | - | 0 |
| 红外导引头 | 100 | - | [见红外导引头算法](#signature-player-ir) |
| 雷达导引头 | 50 | - | [见雷达导引头算法](#signature-player-radar) |
| 激光导引头 | - | 1 | 0 |
| 反辐射导引头 | 250 | - | 100 |

> 说明：`-` 表示该组合不支持或本文档未定义固定值。

#### 2.2.2 对玩家目标时的详细算法（仅红外/雷达导引头）

红外/雷达导引头（玩家飞机）的计算较复杂，会根据玩家飞机状态动态变化。

<a id="signature-player-ir"></a>

###### 红外导引头（玩家目标）

1. 先计算目标红外值 `targetIR`：
   - 有燃油时：遍历当前连接到驾驶舱的所有引擎，累加每种发动机的红外 Signature；
   - 然后乘以 `0.25`；
   - 无燃油时，`targetIR = 0`。
2. 再进行平滑逼近：
   - `IRSignature = StepTowards(IRSignature, 250f * deltaTime, targetIR)`

即：

```math
IR_{target}=
\begin{cases}
0.25\cdot\sum IR_{engine}, & Fuel>0 \\
0, & Fuel\le 0
\end{cases}
```

```math
IR_{new}=StepTowards(IR_{old},\,250\cdot\Delta t,\,IR_{target})
```

各类型发动机的 IRSignature 计算方式：

- 喷气引擎普通状态 IRSignature = 当前节流阀大小 * 功率倍率 * 最大功率 * 1
- 喷气引擎加力燃烧状态 IRSignature = 喷气引擎普通状态 IRSignature * Lerp(1, 10, afterburnerPercent)
- 旋翼/螺旋桨 IRSignature = 喷气引擎普通状态 IRSignature * 0.1
- 车辆引擎 IRSignature = 当前节流阀大小 * 最大功率 * 0.5

加力节流阀计算：

```math
afterburnerPercent=\mathrm{clamp01}\left(\frac{\text{throttle}-\text{AfterburnerThrottleStart}}{1-\text{AfterburnerThrottleStart}}\right)
```

<a id="signature-player-radar"></a>

###### 雷达导引头（玩家目标）

算法：

1. 累加每个部件在六个方向（上下左右前后）阻力之和；
2. 再加上当前机翼表面积。

即：

```math
RadarSignature=\sum_{part}(D_f+D_b+D_l+D_r+D_d+D_u)+WingSurfaceArea
```

注意：

1. 此处“阻力”并非传统空气阻力，更接近有效阻力面积的工程量，因此单位不是牛顿。
2. 部件 XML 属性 `dragScale` 和 `calculateDrag` 也会影响雷达特征强度计算。
3. 由于雷达特征还会计入机翼面积，因此即便把所有部件阻力调到 0，飞机仍会有雷达特征强度；且即便没有机翼，锁定仍有每秒 `0.1` 的保底速率，因此**做不到雷达下的完全隐身**。

---

## 3. 会让锁定“变慢/重置”的额外机制

- 当目标的 `evade/break lock probability` 上升时，会触发一次随机判定；
- 若判定失败，则直接：
  - 锁定进度归零
  - 1.5 秒冷却后才能重新锁定

---

## 4. 非 XML（硬编码/代码常量）的关键项

- 锁定速率限制区间：`0 ~ 2`（后有最低保底 `0.1`）
- 连续锁倍率：`1.5`
- 非锁定时衰减：`0.5/s`
- 干扰后冷却：`1.5s`
