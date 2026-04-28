## Funky Tree 参数清单

### 单位约定（基于源码）

- 角度相关：单位为 **度（°）**。
- 角速度相关：单位为 **度每秒（°/s）**。
- 时间相关：单位为 **秒（s）**
- 距离/高度/坐标相关：使用游戏世界坐标单位（Unity world unit，工程中通常按米理解）。
- 速度相关：世界坐标单位每秒（通常按 **m/s** 理解）。
- `Latitude`/`Longitude` 在该工程里是坐标轴值（`z/x`），**不是地理经纬度“度数”, 游戏中一般按米理解**。

### 常量

| 参数分类 | 参数名称 | 参数说明 | 参数返回什么样的内容 |
|---|---|---|---|
| 常量 | `true` | 布尔真常量 | `bool` |
| 常量 | `false` | 布尔假常量 | `bool` |
| 常量 | `pi` | 圆周率常量 | `number(float)` |
| 常量 | `e` | 当前实现为 `Mathf.Log(1f)`，值为 `0`（注意：不是数学常见的 $e\approx2.718$） | `number(float)` |

### 默认函数（内置）

| 参数分类 | 参数名称 | 参数说明 | 参数返回什么样的内容 |
|---|---|---|---|
| 默认函数 | `abs(x)` | 绝对值，`x:number` | `number(float)` |
| 默认函数 | `acos(x)` | 反余弦，输入 `x:number`（无单位，常见范围 `[-1,1]`），**返回角度制（°）** | `number(float)` |
| 默认函数 | `asin(x)` | 反正弦，输入 `x:number`（无单位，常见范围 `[-1,1]`），**返回角度制（°）** | `number(float)` |
| 默认函数 | `atan(x)` | 反正切，输入 `x:number`（无单位），**返回角度制（°）** | `number(float)` |
| 默认函数 | `atan2(y, x)` | 双参数反正切，`y:number, x:number`（两者同量纲），**返回角度制（°）** | `number(float)` |
| 默认函数 | `ceil(x)` | 向上取整，`x:number`；返回仍是 `float`，但数值是整数值 | `number(float)` |
| 默认函数 | `clamp(value, min, max)` | 限幅，3个参数均为 `number` | `number(float)` |
| 默认函数 | `clamp01(value)` | 限幅到 `[0,1]`，`value:number` | `number(float)` |
| 默认函数 | `cos(angle)` | 余弦，输入 `angle:number`（单位 **°**） | `number(float)` |
| 默认函数 | `deltaangle(current, target)` | 最短角差，`current:number, target:number`（角度，单位 **°**）；返回约在 `[-180, 180]` 的角差 | `number(float)` |
| 默认函数 | `exp(x)` | 自然指数函数，计算 $e^x$（这里的 $e$ 是数学常数，不依赖上下文常量 `e` 的取值） | `number(float)` |
| 默认函数 | `floor(x)` | 向下取整，`x:number`；返回仍是 `float`，但数值是整数值 | `number(float)` |
| 默认函数 | `format(value, format)` | 数值格式化；`value:number, format:string`。若格式首字母是 `D/d/X/x`，源码会先把 `value` 转成 `int` 再格式化 | `string` |
| 默认函数 | `inverselerp(a, b, value)` | 反插值；`a,b,value:number`，返回插值系数 `t`（`Mathf.InverseLerp`，结果会钳制到 `[0,1]`） | `number(float)` |
| 默认函数 | `lerp(a, b, t)` | 线性插值；`a,b,t:number`，其中 `t` 在实现中会钳制到 `[0,1]` | `number(float)` |
| 默认函数 | `lerpangle(a, b, t)` | 角度插值，`a,b` 为角度（单位 **°**），`t` 为无单位插值系数 | `number(float)` |
| 默认函数 | `lerpunclamped(a, b, t)` | 非限幅线性插值，3个参数均为 `number` | `number(float)` |
| 默认函数 | `log(value, base)` | 对数，`value:number, base:number`（对应 `Mathf.Log(value, base)`） | `number(float)` |
| 默认函数 | `log10(x)` | 以10为底对数，`x:number` | `number(float)` |
| 默认函数 | `max(a, b)` | 最大值，`a:number, b:number` | `number(float)` |
| 默认函数 | `min(a, b)` | 最小值，`a:number, b:number` | `number(float)` |
| 默认函数 | `pingpong(t, length)` | 往返波动，`t:number, length:number`；返回值在 `[0, length]` 间往返 | `number(float)` |
| 默认函数 | `pow(value, power)` | 幂运算，`value:number, power:number` | `number(float)` |
| 默认函数 | `repeat(t, length)` | 周期重复，`t:number, length:number`；返回值在 `[0, length)`（对应 `Mathf.Repeat`） | `number(float)` |
| 默认函数 | `round(x)` | 四舍五入到最接近整数，`x:number`；返回仍是 `float` | `number(float)` |
| 默认函数 | `sign(x)` | 符号函数，`x:number`；对应 `Mathf.Sign`，`x >= 0` 返回 `1`，`x < 0` 返回 `-1` | `number(float)` |
| 默认函数 | `sin(angle)` | 正弦，输入 `angle:number`（单位 **°**） | `number(float)` |
| 默认函数 | `smoothstep(from, to, t)` | 平滑插值；`from,to,t:number`，实现会先将 `t` 钳制到 `[0,1]` 再进行平滑插值 | `number(float)` |
| 默认函数 | `sqrt(x)` | 平方根，`x:number` | `number(float)` |
| 默认函数 | `tan(angle)` | 正切，输入 `angle:number`（单位 **°**） | `number(float)` |

### 特殊函数（带记忆状态）

| 参数分类 | 参数名称 | 参数说明 | 参数返回什么样的内容 |
|---|---|---|---|
| 特殊函数 | `sum(value)` | 积分器，`value:number`，按每帧 $\Delta t$（秒）累加：$S\leftarrow S+value\cdot\Delta t$。若 `value` 单位为 `U`，结果单位为 `U·s` | `number(float)` |
| 特殊函数 | `rate(value)` | 微分器，`value:number`，计算变化率：$\frac{value-last}{\Delta t}$。若 `value` 单位为 `U`，结果单位为 `U/s`；首次调用返回 `0` | `number(float)` |
| 特殊函数 | `PID(target, current, p, i, d)` | PID控制输出；源码为：`error = target - current`，`I += error*dt`，`D = (lastCurrent - current)/dt`（首次为0），输出 `p*error + i*I + d*D` | `number(float)` |
| 特殊函数 | `smooth(value, maxRate)` | 速率限制平滑；源码基于 `MoveTowards(last, value, maxRate*dt)`，首次调用直接返回当前 `value` | `number(float)` |

### 飞行状态暴露（`AircraftScript` 的 `[Exposed]`）

| 参数分类 | 参数名称 | 参数说明 | 参数返回什么样的内容 |
|---|---|---|---|
| 飞行状态属性 | `Altitude` | 高度（相对海平面），来自 `GlobalPosition.y - SeaLevel`（世界坐标距离单位，通常按米） | `number(float)` |
| 飞行状态属性 | `AltitudeAgl` | 离地高度（AGL），来自射线距离 `RaycastHit.distance`（世界坐标距离单位，通常按米） | `number(float)` |
| 飞行状态属性 | `Rpm1` | 发动机/通道1转速（RPM，转/分钟） | `number(float)` |
| 飞行状态属性 | `Rpm2` | 发动机/通道2转速（RPM，转/分钟） | `number(float)` |
| 飞行状态属性 | `Rpm3` | 发动机/通道3转速（RPM，转/分钟） | `number(float)` |
| 飞行状态属性 | `Rpm4` | 发动机/通道4转速（RPM，转/分钟） | `number(float)` |
| 飞行状态属性 | `AngleOfAttack` | 迎角（AoA，单位 **°**） | `number(float)` |
| 飞行状态属性 | `AngleOfSlip` | 侧滑角（单位 **°**） | `number(float)` |
| 飞行状态属性 | `Fuel` | 燃油比例（源码别名映射自 `FuelProportion`） | `number(float)` |
| 飞行状态属性 | `GForce` | 总过载（单位 **g**，1g≈9.81m/s²） | `number(float)` |
| 飞行状态属性 | `GS` | 地速（单位：世界坐标速度，通常按 m/s） | `number(float)` |
| 飞行状态属性 | `Heading` | 航向角（单位 **°**） | `number(float)` |
| 飞行状态属性 | `IAS` | 指示空速（单位：世界坐标速度，通常按 m/s） | `number(float)` |
| 飞行状态属性 | `Latitude` | 实际为 `GlobalPosition.z` 坐标值（世界坐标单位，**非地理纬度度数**） | `number(float)` |
| 飞行状态属性 | `Longitude` | 实际为 `GlobalPosition.x` 坐标值（世界坐标单位，**非地理经度度数**） | `number(float)` |
| 飞行状态属性 | `PitchAngle` | 俯仰角（单位 **°**） | `number(float)` |
| 飞行状态属性 | `PitchRate` | 俯仰角速度（单位 **°/s**） | `number(float)` |
| 飞行状态属性 | `RollAngle` | 横滚角（单位 **°**） | `number(float)` |
| 飞行状态属性 | `RollRate` | 横滚角速度（单位 **°/s**） | `number(float)` |
| 飞行状态属性 | `SelectedWeapon` | 当前选中武器名（别名映射自 `SelectedWeaponName`） | `string` |
| 飞行状态属性 | `TargetDistance` | 目标距离（世界坐标距离单位，通常按米） | `number(float)` |
| 飞行状态属性 | `TargetElevation` | 目标仰角/高低角（单位 **°**） | `number(float)` |
| 飞行状态属性 | `TargetHeading` | 目标方位角（单位 **°**） | `number(float)` |
| 飞行状态属性 | `TargetLocked` | 是否已锁定目标 | `bool` |
| 飞行状态属性 | `TargetLocking` | 是否正在锁定目标 | `bool` |
| 飞行状态属性 | `TargetSelected` | 是否已有选中目标 | `bool` |
| 飞行状态属性 | `TAS` | 真空速（单位：世界坐标速度，通常按 m/s） | `number(float)` |
| 飞行状态属性 | `Time` | 飞行时间（别名映射自 `TimeSinceStart`，单位 **s**） | `number(float)` |
| 飞行状态属性 | `VerticalG` | 垂直方向过载（单位 **g**） | `number(float)` |
| 飞行状态属性 | `YawRate` | 偏航角速度（单位 **°/s**） | `number(float)` |
| 飞行状态方法 | `ammo(weapon)` | 查询武器弹药。入参：`weapon:string`（武器名）；返回该武器当前弹药数量（计数值） | `number(float)` |

### 控制输入/上下文变量（`AircraftControls.SetupContext` + 控制面局部）

| 参数分类 | 参数名称 | 参数说明 | 参数返回什么样的内容 |
|---|---|---|---|
| 控制输入变量 | `Trim` | 配平输入 | `number(float)` |
| 控制输入变量 | `Flaps` | 襟翼输入 | `number(float)` |
| 控制输入变量 | `Vtol` | VTOL 过渡输入 | `number(float)` |
| 控制输入变量 | `Roll` | 横滚输入 | `number(float)` |
| 控制输入变量 | `Pitch` | 俯仰输入 | `number(float)` |
| 控制输入变量 | `Yaw` | 偏航输入 | `number(float)` |
| 控制输入变量 | `Brake` | 刹车输入 | `number(float)` |
| 控制输入变量 | `Throttle` | 油门输入 | `number(float)` |
| 控制输入变量 | `GearDown` | 起落架是否放下 | `bool` |
| 控制输入变量 | `LandingGear` | 旧版起落架浮点量（放下=0，收起=1） | `number(float)` |
| 控制输入变量 | `FireGuns` | 机炮开火输入 | `bool` |
| 控制输入变量 | `FireWeapons` | 武器发射输入 | `bool` |
| 控制输入变量 | `LaunchCountermeasures` | 释放干扰弹输入 | `bool` |
| 控制输入变量 | `ParkingBrake` | 停车刹车状态 | `bool` |
| 控制输入变量 | `Activate1` | 激活组1状态 | `bool` |
| 控制输入变量 | `Activate2` | 激活组2状态 | `bool` |
| 控制输入变量 | `Activate3` | 激活组3状态 | `bool` |
| 控制输入变量 | `Activate4` | 激活组4状态 | `bool` |
| 控制输入变量 | `Activate5` | 激活组5状态 | `bool` |
| 控制输入变量 | `Activate6` | 激活组6状态 | `bool` |
| 控制输入变量 | `Activate7` | 激活组7状态 | `bool` |
| 控制输入变量 | `Activate8` | 激活组8状态 | `bool` |
| 控制面局部变量 | `Aileron` | 控制面局部副翼量（考虑机翼翻转方向） | `number(float)` |
| 控制面局部变量 | `WingFlipped` | 机翼翻转方向标志（`-1` 或 `1`） | `number(float)` |

### 事件/信号类参数（`VariableOutput` + 动态声明）

| 参数分类 | 参数名称 | 参数说明 | 参数返回什么样的内容 | 生效零件（来源脚本） |
|---|---|---|---|---|
| 事件/信号 | `Altitude` | 高度输出信号（世界坐标高度单位，通常按米） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号 | `Ammo` | 弹药余量输出（如干扰弹发射器） | `number(float)` | `CounterMeasureDispenserScript`（干扰弹发射器） |
| 事件/信号 | `Current Angle` | 当前角度输出（关节/旋转件，单位 **°**） | `number(float)` | `JointRotatorScript`（关节旋转器） |
| 事件/信号 | `Drag Force` | 阻力大小输出 | `number(float)` | `WingScript`（机翼） |
| 事件/信号 | `Extension` | 悬挂/减震伸缩量 | `number(float)` | `SuspensionScript`（悬挂） |
| 事件/信号 | `Fired` | 发射触发信号（导弹/炸弹，常以 `0/1` 脉冲表示） | `number(float)` | `BombScript`（炸弹）、`MissileScript`（导弹） |
| 事件/信号 | `Forward Slip` | 前向滑移量（轮胎） | `number(float)` | `ResizableWheelScript`（可调车轮）、`Car/JWheelScript`（车辆车轮） |
| 事件/信号 | `Gear` | 当前挡位 | `number(float)` | `Powertrain/JTransmissionScript`（动力总成变速箱） |
| 事件/信号 | `GearRatio` | 当前齿比 | `number(float)` | `Powertrain/JTransmissionScript`（动力总成变速箱） |
| 事件/信号 | `Heading Angle` | 航向角输出（单位 **°**） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号 | `InputTorque` | 输入扭矩 | `number(float)` | `Powertrain/JTransmissionScript`（动力总成变速箱） |
| 事件/信号 | `Is Active` | 激活状态信号（相机视角等，源码为 `0f/1f`） | `number(float)` | `CameraVantageScript`（相机视角） |
| 事件/信号 | `Latitude` | 实际为位置 `z` 坐标输出（世界坐标单位，**非地理纬度度数**） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号 | `Lift Force` | 升力大小输出 | `number(float)` | `WingScript`（机翼） |
| 事件/信号 | `Longitude` | 实际为位置 `x` 坐标输出（世界坐标单位，**非地理经度度数**） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号 | `Look Pitch` | 观察俯仰角输出（单位 **°**） | `number(float)` | `CameraVantageScript`（相机视角） |
| 事件/信号 | `Look Roll` | 观察横滚角输出（单位 **°**） | `number(float)` | `CameraVantageScript`（相机视角） |
| 事件/信号 | `Look Yaw` | 观察偏航角输出（单位 **°**） | `number(float)` | `CameraVantageScript`（相机视角） |
| 事件/信号 | `Offroad` | 越野/离路面状态量 | `number(float)` | `ResizableWheelScript`（可调车轮）、`Car/JWheelScript`（车辆车轮） |
| 事件/信号 | `OutputTorque` | 输出扭矩 | `number(float)` | `Powertrain/JEngineScript`（动力总成发动机）、`Powertrain/JTransmissionScript`（动力总成变速箱） |
| 事件/信号 | `Pitch Angle` | 俯仰角输出（单位 **°**） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号 | `Pitch Rate` | 俯仰角速度输出（单位 **°/s**） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号 | `Roll Angle` | 横滚角输出（单位 **°**） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号 | `Roll Rate` | 横滚角速度输出（单位 **°/s**） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号 | `RPM` | 转速输出（RPM，转/分钟） | `number(float)` | `BladedEngineScript`（桨叶发动机）、`CarEngineScript`（汽车发动机）、`HeliMainRotorScript`（直升机主旋翼）、`ResizableWheelScript`（可调车轮）、`Car/JWheelScript`（车辆车轮）、`Powertrain/JEngineScript`（动力总成发动机） |
| 事件/信号 | `Sideways Slip` | 侧向滑移量（轮胎） | `number(float)` | `ResizableWheelScript`（可调车轮）、`Car/JWheelScript`（车辆车轮） |
| 事件/信号 | `Speed` | 速度输出（世界坐标速度单位，通常按 m/s） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号 | `Thrust` | 推力输出 | `number(float)` | `EngineScript`（发动机基类）及其派生发动机零件 |
| 事件/信号 | `View Offset X` | 视角偏移 X（位置偏移量，世界/局部坐标单位，通常按米） | `number(float)` | `CameraVantageScript`（相机视角） |
| 事件/信号 | `View Offset Y` | 视角偏移 Y（位置偏移量，世界/局部坐标单位，通常按米） | `number(float)` | `CameraVantageScript`（相机视角） |
| 事件/信号 | `View Offset Z` | 视角偏移 Z（位置偏移量，世界/局部坐标单位，通常按米） | `number(float)` | `CameraVantageScript`（相机视角） |
| 事件/信号 | `Yaw Rate` | 偏航角速度输出（单位 **°/s**） | `number(float)` | `CockpitScript`（座舱） |
| 事件/信号（动态声明） | `<自定义变量名>` | 非固定标签：变量名来自零件配置（通常取输入ID；若含 `:` 只取前缀）。因此不会出现在固定 `[VariableOutput]` 列表里 | `number(float)` | `CockpitButtonScript`（座舱按钮）、`CockpitSwitchScript`（座舱开关） |
| 事件/信号（动态声明） | `<轴变量名>` | 非固定标签：来自 XR 控件轴的 `Variable.Name`（由 `ControlBase` 轴配置动态决定） | `number(float)` | `XR/ControlBaseScript`（XR 控件基座） |

---

## 使用备注（建议放在文档页尾）

- 参数名建议按源码大小写使用（表达式上下文是按字符串键注册）。
- 事件/信号类参数是轮询值，不是 `onEvent()` 回调。
- 除固定 `[VariableOutput]` 标签外，部分零件通过 `IVariableDeclarations` 动态声明变量名；这类名称由零件配置决定，不会提前固化在静态标签清单中。
- `VariableOutput` 中仅少数有默认变量映射（例如 `RotorRPM`）；多数需要在变量输出配置里手动命名后再引用。

## 本轮进度更新

- ✅ 已核对 `[Exposed]` 成员真实类型与方法入参  
- ✅ 已核对 `Context` 默认常量/函数签名  
- ✅ 已核对 `SpecialFunctions` 参数与返回  
- ✅ 已核对 `VariableOutput` 标签对应输出类型（均为 `float`）

如果你需要，我下一步可以把这份表直接整理成 `Markdown` 文件（例如 `Game/Todo/funky-tree-参数总表.md`），并再附一版英文对照列。