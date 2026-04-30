## 零件 XML 属性文档
- 零件总数: 83
- 属性行总数: 654
- 无独有属性零件数: 5

## 提示:

- 该文档由 AI 捞取后生成，字段描述可能存在错误或偏差。
- bool类型数值写为true/false
- 枚举类型在xml中应写为字符串，保持大小写和原有枚举对象一致，如文档中提供枚举“枚举(CannonData.ProjectileStyle: Sphere、Slug)”，则xml中应写为“Sphere”或“Slug”，而非全小写或其他变体。

## 属性列表

| 零件类别 | 零件类名 | 属性名 | 作用说明 | 输入类型 |
| --- | --- | --- | --- | --- |
| Advanced Performance Scalars | RotorPerfScalarsData | collectiveDrag | 主旋翼总距对应的阻力缩放系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | collectiveLift | 主旋翼总距对应的升力缩放系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | collectiveTorque | 主旋翼总距对应的扭矩缩放系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicMotorDragTorque | 周期操纵引起的电机阻力扭矩缩放 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicPitchInputExpo | 周期俯仰输入指数曲线 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicRollInputExpo | 周期横滚输入指数曲线 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicRpmFalloffExpo | 周期操纵随转速衰减的指数曲线 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicStrength | 周期操纵总体强度系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | groundEffect | 地面效应增益系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | gyroscopicLag | 旋翼陀螺响应滞后系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | gyroscopicStabilization | 旋翼陀螺稳定系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | relativeWindPassiveLift | 相对风被动升力系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | relativeWindPassiveTorque | 相对风被动扭矩系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | relativeWindPeakSpeed | 相对风效应峰值速度 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | rotorTensor | 旋翼转动惯量系数 | float |
| Advanced Performance Scalars | RotorPerfScalarsData | translationalLift | 平移升力系数 | float |
| Airbrake | AirBrakeData | drag | 空气刹车阻力系数 | float |
| Arresting Hook | ArrestingHookData | activationGroup | 设置功能所属激活组，用于按键触发开关 | string (1~8) |
| Arresting Hook | ArrestingHookData | cableDeceleration | 拦阻索对机体的减速度系数 | float |
| Arresting Hook | ArrestingHookData | deployedAngle | 拦阻钩放下角度（度） | float |
| Attitude Ball | AttitudeBallData | meshPath | 目标网格路径 | string |
| Attitude Ball | AttitudeBallData | rotationType | 姿态球旋转模式（按所选轴组合旋转） | 枚举(AttitudeBallData.BallType: 无、Roll、Pitch、Heading、Attitude、LevelCompass、AllAxis) |
| Attitude Ball | AttitudeBallData | scale | 缩放系数 | float |
| Beacon Light | BeaconLightData | activationGroup | 设置功能所属激活组，用于按键触发开关 | int (0~8，0=All) |
| Beacon Light | BeaconLightData | blinkProgram | 信标灯闪烁时序（每段持续时间，单位秒，逗号分隔） | float列表(逗号分隔秒值) |
| Beacon Light | BeaconLightData | designerBlinkProgram | 设计器使用的闪烁预设样式 | 枚举(预设: Steady、Slow Blink、Quick Blink) |
| Beacon Light | BeaconLightData | input | 输入轴/按钮ID | string |
| Beacon Light | BeaconLightData | intensity | 效果强度 | float |
| Beacon Light | BeaconLightData | showHalo | 是否显示信标灯光晕效果 | bool |
| Bomb | BombData | （无） | 该零件未在自身State中读取独有属性，主要沿用父类或公共层逻辑 | 无 |
| Button | CockpitButtonData | depthBase | 按钮基座深度 | float |
| Button | CockpitButtonData | depthOff | 按钮未按下时深度 | float |
| Button | CockpitButtonData | depthOn | 按钮按下时深度 | float |
| Button | CockpitButtonData | disableTooltip | 是否禁用按钮提示文本 | bool |
| Button | CockpitButtonData | height | 控件高度 | float |
| Button | CockpitButtonData | inputId | 按钮绑定输入ID | string |
| Button | CockpitButtonData | lightStrength | 按钮灯光亮度强度 | float |
| Button | CockpitButtonData | lightTransitionDelay | 按钮灯光变化延迟 | float |
| Button | CockpitButtonData | lightTransitionTime | 按钮灯光变化时长 | float |
| Button | CockpitButtonData | outputValue | 按钮输出值 | float |
| Button | CockpitButtonData | padding | 按钮内边距 | float |
| Button | CockpitButtonData | positionTransitionDelay | 按钮位移动画延迟 | float |
| Button | CockpitButtonData | positionTransitionTime | 按钮位移动画时长 | float |
| Button | CockpitButtonData | style | 按钮外观样式 | 枚举(CockpitButtonStyle: Rectangular、Circular) |
| Button | CockpitButtonData | tooltip | 按钮提示文本 | string |
| Button | CockpitButtonData | width | 宽度 | float |
| Cannon | CannonData | activationGroup | 设置功能所属激活组，用于按键触发开关 | string (0/1~8，0=All) |
| Cannon | CannonData | ammoCount | 机炮弹药总数 | int |
| Cannon | CannonData | barrelLength | 炮管长度 | float |
| Cannon | CannonData | barrelRecoil | 炮管后坐行程系数 | float |
| Cannon | CannonData | baseLength | 炮座长度 | float |
| Cannon | CannonData | diameter | 机炮口径/直径 | float |
| Cannon | CannonData | explosionScalar | 爆炸伤害倍率 | float |
| Cannon | CannonData | firingDelay | 机炮最小射击间隔 | float |
| Cannon | CannonData | flashScale | 枪口闪光缩放 | float |
| Cannon | CannonData | flashSpace | 枪口闪光粒子模拟空间 | 枚举(ParticleSystemSimulationSpace: Local、World、Custom；Custom会回落为Local) |
| Cannon | CannonData | function | 武器用途模式（空对空/空对地/多用途） | 枚举(WeaponFunction: 无、AirToAir、AirToSurface、MultiRole) |
| Cannon | CannonData | fuseInput | 引信触发表达式 | string |
| Cannon | CannonData | impactDamageScalar | 撞击命中伤害倍率 | float |
| Cannon | CannonData | launchVolume | 发射音量 | float |
| Cannon | CannonData | muzzleBrake | 是否启用炮口制退器 | bool |
| Cannon | CannonData | name | 自定义名称 | string |
| Cannon | CannonData | projectileLifetime | 弹丸生命周期（秒） | float |
| Cannon | CannonData | projectileStyle | 弹丸几何外形样式 | 枚举(CannonData.ProjectileStyle: Sphere、Slug) |
| Cannon | CannonData | projectileType | 弹丸伤害类型 | 枚举(CannonData.ProjectileType: Basic、Explosive) |
| Cannon | CannonData | projectileVelocity | 弹丸初速度 | float |
| Cannon | CannonData | recoilForce | 后坐力系数 | float |
| Cannon | CannonData | tracerColor | 曳光弹颜色 | Color(HTML Hex #RRGGBB/#RRGGBBAA) |
| Cannon | CannonData | tracerLength | 曳光长度 | float |
| Cannon | CannonData | tracerSpacing | 曳光间隔（每N发） | int |
| Canopy | CanopyData | activationGroup | 设置功能所属激活组，用于按键触发开关 | int (0~8) |
| Canopy | CanopyData | animationPath | 舱盖动画节点路径 | string |
| Canopy | CanopyData | animationSpeed | 舱盖动画播放速度 | float |
| Canopy | CanopyData | dragWhenOpen | 舱盖打开时附加阻力 | float |
| Canopy | CanopyData | insideSubmesh | 舱盖内侧使用的子网格索引 | int |
| Canopy | CanopyData | meshPath | 目标网格路径 | string |
| Canopy | CanopyData | name | 自定义名称 | string |
| Canopy | CanopyData | opacity | 透明度 | float |
| Canopy | CanopyData | outsideSubmesh | 舱盖外侧使用的子网格索引 | int |
| Canopy | CanopyData | showInside | 是否显示舱盖内侧玻璃 | bool |
| Car Engine | CarEngineData | fuelConsumptionRate | 燃油消耗速率 | float |
| Car Engine | CarEngineData | power | 功率/推力强度 | float |
| Car Engine | CarEngineData | throttleResponse | 油门响应速度 | float |
| Catapult Connector | CatapultConnectorData | catapultAcceleration | 弹射器加速度倍率 | float |
| Catapult Connector | CatapultConnectorData | targetLaunchSpeed | 目标弹射离舰速度 | float |
| Cockpit | CockpitData | hasCamera | 该座舱是否提供相机视角 | bool |
| Cockpit | CockpitData | lookBackTranslation | 座舱后视时相机平移偏置 | Vector2(x,y) |
| Cockpit | CockpitData | primaryCockpit | 是否设为主座舱 | bool |
| Cockpit Sound | CockpitSoundData | activationGroup | 设置功能所属激活组，用于按键触发开关 | string (AlwaysOn、AlwaysOff、1~8) |
| Cockpit Sound | CockpitSoundData | intensity | 效果强度 | float |
| Control Base | ControlBaseData | attachPointId | Joint模式下控制基座绑定的连接点ID | int |
| Control Base | ControlBaseData | axis | 控制轴方向向量 | Vector3(x,y,z) |
| Control Base | ControlBaseData | haptics | 是否启用触觉反馈 | bool |
| Control Base | ControlBaseData | ignoreAircraftCollisions | 控制基座是否忽略与本机碰撞 | bool |
| Control Base | ControlBaseData | input | 输入轴/按钮ID | string |
| Control Base | ControlBaseData | max | 轴向输入上限 | float |
| Control Base | ControlBaseData | min | 轴向输入下限 | float |
| Control Base | ControlBaseData | mode | 控制基座模式（关节驱动或目标变换驱动） | 枚举(ControlMode: Joint、Transform) |
| Control Base | ControlBaseData | name | 自定义名称 | string |
| Control Base | ControlBaseData | positionDamper | 平移驱动阻尼 | float |
| Control Base | ControlBaseData | positionMaximumForce | 平移驱动最大力 | float |
| Control Base | ControlBaseData | positionSpring | 平移驱动弹簧刚度 | float |
| Control Base | ControlBaseData | rotationMaxDistance | 旋转轴最大偏转距离 | float |
| Control Base | ControlBaseData | scale | 缩放系数 | float |
| Control Base | ControlBaseData | slerpDamper | 角度驱动阻尼 | float |
| Control Base | ControlBaseData | slerpMaximumForce | 角度驱动最大力 | float |
| Control Base | ControlBaseData | slerpSpring | 角度驱动弹簧刚度 | float |
| Control Base | ControlBaseData | targetTransformPath | Transform模式目标节点路径 | string |
| Control Base | ControlBaseData | v | 状态版本号 | int |
| Control Surface | ControlSurfacePartData | dummyPartFlipped | 控制面镜像时是否翻转 | bool |
| Control Surface | ControlSurfacePartData | dummyWingOffset | 控制面关联机翼的偏移缓存 | Vector2(x,y) |
| Control Surface | ControlSurfacePartData | dummyWingScale | 控制面关联机翼的缩放缓存 | Vector2(x,y) |
| Control Surface | ControlSurfacePartData | style | 样式方案 | string |
| Countermeasure Dispenser | CounterMeasureDispenserData | activationGroup | 设置功能所属激活组，用于按键触发开关 | int |
| Countermeasure Dispenser | CounterMeasureDispenserData | ammo | 反制措施可用数量 | int |
| Countermeasure Dispenser | CounterMeasureDispenserData | autoDispenseDelay | 自动释放反制措施的间隔时间（秒） | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | breakLockChance | 干扰后使导弹断开锁定的概率 | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | evadeLockChance | 干扰后规避锁定的概率 | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | launchForce | 反制弹发射力 | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | type | 反制措施类型 | 枚举(CounterMeasureType: 无、Flares、Chaff) |
| Decal | DecalData | color | 贴花颜色（Tint） | Color(HEX RGB) |
| Decal | DecalData | decalRotation | 贴花欧拉旋转角 | Vector3(x,y,z) |
| Decal | DecalData | opacity | 透明度 | float |
| Decal | DecalData | partIds | 目标零件ID列表 | int列表(逗号分隔) |
| Decal | DecalData | penetration | 贴花投射深度/穿透系数 | float |
| Decal | DecalData | priority | 贴花渲染优先级 | int |
| Decal | DecalData | size | 尺寸比例 | Vector3(x,y,z) |
| Decal | DecalData | target | 贴花目标模式 | string (Single Part/MultipleParts) |
| Decal | TextureDecalData | decalId | 贴花纹理ID | string |
| Decal | TextureDecalData | offset | 位置偏移向量 | Vector2(x,y) |
| Decal | TextureDecalData | tiling | 贴花平铺倍率 | Vector2(x,y) |
| Detacher | DetacherData | attachPointsToDetach | 触发分离时要断开的连接点ID列表 | int列表(逗号分隔) |
| Detacher | DetacherData | delay | 分离触发延迟（秒） | float |
| Detacher | DetacherData | detacherUiMaxForce | 分离器UI可调的最大分离力 | float |
| Detacher | DetacherData | detachForce | 实际施加的分离力 | float |
| Detacher | DetacherData | direction | 分离施力方向 | 枚举(DetacherDirection: Default、Forward) |
| Detacher | DetacherData | enabled | 是否启用该功能 | bool |
| Detacher | DetacherData | group | 分离器所属激活组 | string (0/1~8，0=Disabled) |
| Differential | JDifferentialData | coastStiffness | 差速器在收油/制动状态下的锁止响应 | float |
| Differential | JDifferentialData | lock | 差速器锁止比例 | float |
| Differential | JDifferentialData | powerStiffness | 差速器在加速状态下的锁止响应 | float |
| Differential | JDifferentialData | size | 尺寸比例 | float |
| Drive Shaft | JDriveHubData | reversed | 是否反转旋转方向 | bool |
| Drive Shaft | JDriveShaftData | bootA | 是否显示传动轴A端防尘套 | bool |
| Drive Shaft | JDriveShaftData | bootB | 是否显示传动轴B端防尘套 | bool |
| Drive Shaft | JDriveShaftData | end | 传动轴终点局部坐标 | Vector3(x,y,z) |
| Drive Shaft | JDriveShaftData | radius | 半径 | float |
| Drive Shaft | JDriveShaftData | start | 传动轴起点局部坐标 | Vector3(x,y,z) |
| Drive Shaft | JDriveShaftData | visual | 是否显示可视化传动轴 | bool |
| Engine | EngineData | alphaTiedToThrottle | 尾焰透明度是否随油门变化 | bool |
| Engine | EngineData | ductedThrust | 是否按涵道推力模式计算 | bool |
| Engine | EngineData | exhaustScale | 尾焰特效缩放 | Vector3(x,y,z) |
| Engine | EngineData | fuelConsumptionRate | 燃油消耗速率 | float |
| Engine | EngineData | power | 功率/推力强度 | float |
| Engine | EngineData | powerMultiplier | 功率倍率 | float |
| Engine | EngineData | requiredAirIntake | 达到额定输出所需进气量 | float |
| Engine | EngineData | soundOverride | 引擎音效覆盖ID | string |
| Engine | EngineData | throttleResponse | 油门响应速度 | float |
| Engine | EngineData | type | 引擎实现类型 | 枚举(EngineType: Prop、Turbojet、AfterburningTurbojet) |
| Engine | JEngineData | basePower | 引擎基础功率标定值 | float |
| Engine | JEngineData | baseRpm | 引擎基础转速标定值 | float |
| Engine | JEngineData | baseSize | 引擎基础尺寸标定值 | float |
| Engine | JEngineData | cylinderRows | 每列（或每组）气缸数量 | int |
| Engine | JEngineData | engineConfiguration | 发动机构型索引（缸型配置） | int |
| Engine | JEngineData | engineTuning | 发动机调校倾向（扭矩↔高转） | float |
| Engine | JEngineData | forcedInduction | 增压强度（强制进气比例） | float |
| Engine | JEngineData | horsePower | 发动机马力 | float |
| Engine | JEngineData | mass | 发动机质量 | float |
| Engine | JEngineData | massToPower | 功重比系数 | float |
| Engine | JEngineData | powerCurve | 发动机动力曲线（序列化字符串） | string |
| Engine | JEngineData | redLine | 红线转速比例 | float |
| Engine | JEngineData | rpm | 发动机最大转速 | float |
| Engine | JEngineData | rpmScalingExponent | 尺寸对转速影响的缩放指数 | float |
| Engine | JEngineData | size | 尺寸比例 | float |
| Engine | JEngineData | soundPitchLimit | 声音音高上限 | float |
| Engine | JEngineData | soundPitchOffset | 声音音高偏移 | float |
| Engine | JEngineData | soundPitchRange | 声音音高变化范围 | float |
| Engine | JEngineData | soundType | 引擎声音类型组合 | 枚举(EngineSoundType: 无、Prop、Car、Boat、V、Flat、Radial、Inline、Electric、PropV、PropFlat、PropRadial、CarV、CarFlat、CarInline) |
| Engine | JEngineData | startupDuration | 发动机启动时长 | float |
| Engine | JEngineData | supercharger | 是否启用机械增压 | bool |
| Engine | JEngineData | superchargerMultiplier | 机械增压倍率 | float |
| Engine | JEngineData | throttleResponse | 油门响应速度 | float |
| Floating Part | FloatingPartData | enabled | 是否启用该功能 | bool |
| Floating Part | FloatingPartData | impactVelocityAdjustment | 入水冲击速度修正曲线（名称或常数） | string (曲线名或单一浮点值) |
| Floating Part | FloatingPartData | reduceBuoyancyIfBySelf | 自身包围水体时是否降低浮力 | bool |
| Floating Part | FloatingPartData | weightFactor | 浮力重量系数 | float |
| Fuel Tank | FuelTankData | capacity | 油箱最大容量 | float |
| Fuel Tank | FuelTankData | fuel | 当前燃油量 | float |
| Fuel Tank | ResizableFuelTankData | capacity | 油箱最大容量 | float |
| Fuel Tank | ResizableFuelTankData | size | 尺寸比例 | float |
| Fuselage | FuselageData | autoSizeOnConnected | 与其它机身连接时是否自动匹配截面尺寸 | bool |
| Fuselage | FuselageData | buoyancy | 零件浮力系数 | float |
| Fuselage | FuselageData | collider | 机身碰撞体生成模式 | 枚举(FuselageColliderType: Auto、Basic、ConvexMesh、NonConvexMesh) |
| Fuselage | FuselageData | collider | 碰撞体生成模式 | 枚举(FuselageData.FuselageColliderType: Auto、Basic、ConvexMesh、NonConvexMesh) |
| Fuselage | FuselageData | cornerTypes | 机身角类型列表（前后截面） | int列表(8项，逗号分隔) |
| Fuselage | FuselageData | deadWeight | 附加载荷质量 | float |
| Fuselage | FuselageData | fillBack | 机身后截面裁切参数（支持单值或四向值） | float 或 float4(top,bottom,left,right) |
| Fuselage | FuselageData | fillCutFace | 裁切后是否封口 | bool |
| Fuselage | FuselageData | fillFront | 机身前截面裁切参数（支持单值或四向值） | float 或 float4(top,bottom,left,right) |
| Fuselage | FuselageData | frontScale | 机身前截面缩放 | Vector2(x,y) |
| Fuselage | FuselageData | fuelPercentage | 机身可用燃油占比 | float |
| Fuselage | FuselageData | inletSlant | 进气口倾斜角 | float |
| Fuselage | FuselageData | inletThicknessFront | 进气前缘厚度 | float |
| Fuselage | FuselageData | inletThicknessRear | 进气后缘厚度 | float |
| Fuselage | FuselageData | inletTrimSize | 进气口饰边尺寸 | float |
| Fuselage | FuselageData | offset | 位置偏移 | Vector3(x,y,z) |
| Fuselage | FuselageData | rearScale | 机身后截面缩放 | Vector2(x,y) |
| Fuselage | FuselageData | smoothBack | 后段法线平滑开关 | bool |
| Fuselage | FuselageData | smoothFront | 前段法线平滑开关 | bool |
| Fuselage | FuselageData | type | 机身类型标识（机身/锥体/进气道/中空/玻璃等） | string (body、cone、inlet、hollow、glass、hollowglass) |
| Fuselage | FuselageData | version | 状态版本号 | int |
| Fuselage | JFuselageData | autoResize | 连接时是否自动调整机身截面尺寸 | bool |
| Fuselage | JFuselageData | buoyancy | 浮力系数 | float |
| Fuselage | JFuselageData | colliderCornerSamples | 碰撞体角点采样数 | int |
| Fuselage | JFuselageData | cornerRadii | 机身截面四角圆角半径 | Vector4(x,y,z,w) |
| Fuselage | JFuselageData | cornerSamples | 机身截面四角采样数 | Int4(x,y,z,w) |
| Fuselage | JFuselageData | cornerStretch | 机身截面角点拉伸开关 | Bool4(x,y,z,w) |
| Fuselage | JFuselageData | cutting | 机身截面裁切参数 | decimal?列表(4项，逗号分隔，可留空) |
| Fuselage | JFuselageData | deadMassKg | 附加死重（kg） | float |
| Fuselage | JFuselageData | defaultThicknessFront | 前截面默认厚度 | float |
| Fuselage | JFuselageData | defaultThicknessRear | 后截面默认厚度 | float |
| Fuselage | JFuselageData | edgeCurvature | 机身截面边缘曲率 | Vector4(x,y,z,w) |
| Fuselage | JFuselageData | edgeSamples | 机身截面边缘采样数 | Int4(x,y,z,w) |
| Fuselage | JFuselageData | fuelProportion | 燃油占容积比例 | float |
| Fuselage | JFuselageData | glass | 是否启用玻璃材质模式 | bool |
| Fuselage | JFuselageData | legacyThickness | 是否使用旧版厚度逻辑 | bool |
| Fuselage | JFuselageData | mass | 序列化质量与重心打包值（x,y,z,mass） | Vector4(x,y,z,w) |
| Fuselage | JFuselageData | noseconeRoundness | 锥鼻圆润程度 | float |
| Fuselage | JFuselageData | numColliders | 碰撞体分段数量 | int |
| Fuselage | JFuselageData | offset | 位置偏移 | Vector3(x,y,z) |
| Fuselage | JFuselageData | size | 机身截面尺寸（SectionA/SectionB） | Vector2(x,y) |
| Fuselage | JFuselageData | smoothing | 截面平滑开关 | bool |
| Fuselage | JFuselageData | style | 样式类型 | 枚举(FuselageStyle: Body、Hollow、Inlet、Cone、HollowCone) |
| Fuselage | JFuselageData | syncSlices | 前后截面参数是否同步 | bool |
| Fuselage | JFuselageData | thickness | 截面厚度 | float |
| Fuselage | JFuselageData | trapezium | 截面梯形偏置 | float |
| Fuselage | JFuselageData | version | 状态版本号 | int |
| Gauge | GaugeData | altitudeUnit | 高度表单位设置 | 枚举(GaugeData.AltitudeUnit: Feet、Meters、无) |
| Gauge | GaugeData | face | 仪表盘面样式 | 枚举(GaugeData.GaugeFaceTypes: AirSpeed200Indicator、AirSpeed400Indicator、AirSpeed600Indicator、AltimeterIndicator、AttitudeIndicator、FuelIndicator、HeadingIndicator、ThrottleIndicator、TrimIndicator、TurnCoordinatorIndicator、VerticalSpeedIndicator、VTOLIndicator、RotorRPM、Basic1) |
| Gauge | GaugeData | faceEmission | 旧版兼容：统一表盘发光强度 | float |
| Gauge | GaugeData | faceEmissionDay | 表盘白天发光强度 | float |
| Gauge | GaugeData | faceEmissionNight | 表盘夜间发光强度 | float |
| Gauge | GaugeData | faceInput | 表盘面旋转输入表达式 | string |
| Gauge | GaugeData | faceMultiplier | 表盘面输入倍率 | float |
| Gauge | GaugeData | faceZero | 表盘面零位角偏移 | float |
| Gauge | GaugeData | hideBase | 是否隐藏仪表底座 | bool |
| Gauge | GaugeData | hideFace | 是否隐藏仪表盘面 | bool |
| Gauge | GaugeData | hideTrim | 是否隐藏仪表饰圈 | bool |
| Gauge | GaugeData | indicator | 旧版兼容：指针样式 | 枚举(GaugeData.IndicatorType: Indicator1、Indicator2、Indicator3、Indicator4、Indicator5、Indicator6、Indicator7、无) |
| Gauge | GaugeData | indicatorZero | 旧版兼容：指针零位角 | float |
| Gauge | GaugeData | input | 旧版兼容：指针输入源 | string |
| Gauge | GaugeData | invert | 旧版兼容：输入是否反向 | bool |
| Gauge | GaugeData | multiplier | 旧版兼容：输入倍率 | float |
| Gauge | GaugeData | rotationType | 旋转模式 | 枚举(GaugeData.GaugeRotationType: Indicator、Face) |
| Gauge | GaugeData | scale | 缩放系数 | float |
| Gauge | GaugeData | speedUnit | 速度单位设置 | 枚举(GaugeData.SpeedUnit: Knots、MetersPerSecond、MilesPerHour、KilometersPerHour、无) |
| Gauge | GaugeData | trimType | 仪表饰圈样式 | 枚举(GaugeData.GaugeTrimType: Trim1、Trim2) |
| Gauge | GaugeData | type | 类型参数 | 枚举(GaugeData.GaugeTypePreset: Custom、Heading、Fuel、Throttle、Speed200、Speed400、Speed600、Altitude、Trim、TurnCoordinator、VerticalSpeed、RotorRPM、VTOL、BankAngle) |
| Gauge | GaugeData | zero | 旧版兼容：输入零位偏置 | float |
| Gearbox | JGearboxData | gearRatio | 齿轮传动比 | float |
| Gearbox | JGearboxData | reversed | 是否反转输出方向 | bool |
| Gearbox | JGearboxData | size | 尺寸比例 | float |
| Gun | GunData | activationGroup | 设置功能所属激活组，用于按键触发开关 | string (All、1~8) |
| Gun | GunData | ammoCount | 武器弹药总数 | int |
| Gun | GunData | bulletScale | 子弹模型缩放 | Vector3(x,y,z) |
| Gun | GunData | burstCount | 每轮连发数量 | int |
| Gun | GunData | damage | 单发伤害 | float |
| Gun | GunData | impactForce | 命中冲击力 | float |
| Gun | GunData | lifetime | 弹丸生命周期（秒） | float |
| Gun | GunData | muzzleFlash | 是否启用枪口火焰 | bool |
| Gun | GunData | muzzleVelocity | 初速 | float |
| Gun | GunData | roundsPerSecond | 每秒射速 | float |
| Gun | GunData | spread | 散布角 | float |
| Gun | GunData | timeBetweenBursts | 连发间隔时间 | float |
| Gun | GunData | tracerIntensity | 曳光强度 | float |
| Gyroscope | GyroscopeData | activationGroup | 设置功能所属激活组，用于按键触发开关 | string (无、1~8) |
| Gyroscope | GyroscopeData | autoOrient | 是否启用自动姿态保持 | bool |
| Gyroscope | GyroscopeData | pitchRange | 俯仰稳定范围 | float |
| Gyroscope | GyroscopeData | rollRange | 横滚稳定范围 | float |
| Gyroscope | GyroscopeData | speed | 响应速度参数 | float |
| Gyroscope | GyroscopeData | stability | 稳定系数 | float |
| Gyroscope | GyroscopeData | yawPower | 偏航控制强度 | float |
| IK Target | IKTargetData | offset | 位置偏移 | Vector3(x,y,z) |
| IK Target | IKTargetData | path | 目标节点路径 | string |
| IK Target | IKTargetData | positionWeight | IK位置权重 | float |
| IK Target | IKTargetData | priority | 优先级 | int |
| IK Target | IKTargetData | rotationWeight | IK旋转权重 | float |
| IK Target | IKTargetData | type | 类型参数 | 枚举(IKTargetType: Body、LeftShoulder、RightShoulder、LeftThigh、RightThigh、LeftHand、RightHand、LeftFoot、RightFoot、LeftElbow、RightElbow、LeftKnee、RightKnee) |
| Inlet | InletData | airIntakeMultiplier | 进气效率倍率 | float |
| Input Controller | InputControllerData | activationGroup | 设置功能所属激活组，用于按键触发开关 | string (0~8) |
| Input Controller | InputControllerData | defaultActivationGroup | 默认激活组（作为零件初始值） | string (0~8) |
| Input Controller | InputControllerData | defaultInput | 默认输入通道（作为零件初始值） | string |
| Input Controller | InputControllerData | defaultMax | 默认输出上限（作为零件初始值） | float |
| Input Controller | InputControllerData | defaultMin | 默认输出下限（作为零件初始值） | float |
| Input Controller | InputControllerData | input | 输入轴/按钮ID | string |
| Input Controller | InputControllerData | invert | 输入是否反向 | bool |
| Input Controller | InputControllerData | invertOnMirror | 镜像复制时是否反转输入 | bool |
| Input Controller | InputControllerData | invertType | 反转作用方式 | 枚举(InvertType: Axis、Output) |
| Input Controller | InputControllerData | max | 最大输出值 | float |
| Input Controller | InputControllerData | min | 最小输出值 | float |
| Input Controller | InputControllerData | name | 名称标识 | string |
| Input Controller | InputControllerData | propertyEditorDesc | 属性面板显示说明 | string |
| Input Controller | InputControllerData | zeroOnDeactivate | 停用激活组时是否归零输出 | bool |
| Jet Engine | JetEngineData | afterburner | 是否启用加力燃烧室 | bool |
| Jet Engine | JetEngineData | afterburnerBaseColor | 加力尾焰根部颜色 | Color(HTML Hex RGBA) |
| Jet Engine | JetEngineData | afterburnerThrottleStart | 加力介入油门阈值 | float |
| Jet Engine | JetEngineData | afterburnerTipColor | 加力尾焰尖端颜色 | Color(HTML Hex RGBA) |
| Jet Engine | JetEngineData | baseSize | 基础尺寸缩放基准 | float |
| Jet Engine | JetEngineData | burnerTemp | 燃烧室温度设定 | float |
| Jet Engine | JetEngineData | burnerTempRange | 燃烧室温度可调范围 | float列表(2项: min,max) |
| Jet Engine | JetEngineData | bypassRange | 涵道比可调范围 | float列表(2项: min,max) |
| Jet Engine | JetEngineData | bypassRatio | 涵道比 | float |
| Jet Engine | JetEngineData | compressionRange | 压缩比可调范围 | float列表(2项: min,max) |
| Jet Engine | JetEngineData | compressionRatio | 压缩比 | float |
| Jet Engine | JetEngineData | coreVisualScale | 发动机核心可视缩放 | float |
| Jet Engine | JetEngineData | fanPressureRatio | 风扇压比 | float |
| Jet Engine | JetEngineData | fanStyle | 风扇样式ID | string |
| Jet Engine | JetEngineData | gimbalSpeed | 喷口万向摆动速度 | float |
| Jet Engine | JetEngineData | inletConeStyle | 进气锥样式ID | string |
| Jet Engine | JetEngineData | jetEngineType | 喷气发动机类型 | 枚举(JetEngineType: 无、Legacy、Civilian、Military) |
| Jet Engine | JetEngineData | mass | 质量参数 | float |
| Jet Engine | JetEngineData | maxGimbalAngle | 最大喷口偏转角比例 | float |
| Jet Engine | JetEngineData | nozzleLength | 喷口长度系数 | float |
| Jet Engine | JetEngineData | nozzleStyle | 喷口样式ID | string |
| Jet Engine | JetEngineData | reverseThrust | 是否启用反推 | bool |
| Jet Engine | JetEngineData | size | 尺寸比例 | float |
| Jet Engine | JetEngineData | sizeRange | 尺寸可调范围 | float列表(2项: min,max) |
| Jet Engine | JetEngineData | turbinePressureRatio | 涡轮压比 | float |
| Jet Engine Shroud | JetEngineShroudData | jetEngineType | 喷气发动机类型 | 枚举(JetEngineType: 无、Legacy、Civilian、Military) |
| Jet Engine Shroud | JetEngineShroudData | length | 长度系数 | float |
| Jet Engine Shroud | JetEngineShroudData | radius | 半径参数 | float |
| Jet Engine Shroud | JetEngineShroudData | style | 样式类型 | string |
| Joint Motor | JointMotorData | attachPoint | 关节电机绑定连接点索引 | int |
| Joystick | AdjustableJoystickData | colliderPath | 摇杆碰撞体节点路径 | string |
| Joystick | AdjustableJoystickData | cylinderPath | 摇杆杆体节点路径 | string |
| Joystick | AdjustableJoystickData | headPaths | 摇杆头部节点路径列表 | string列表(逗号分隔节点路径) |
| Joystick | AdjustableJoystickData | height | 高度参数 | float |
| Label | LabelData | curvature | 文字弯曲角度 | float |
| Label | LabelData | curvatureDirection | 文字弯曲方向 | 枚举(LabelCurvatureDirection: Horizontal、Vertical) |
| Label | LabelData | designText | 标签显示文本 | string |
| Label | LabelData | emission | 旧版兼容：统一自发光强度 | float |
| Label | LabelData | emissionDay | 白天自发光强度 | float |
| Label | LabelData | emissionNight | 夜间自发光强度 | float |
| Label | LabelData | fontName | 字体名称 | string |
| Label | LabelData | fontSize | 字体大小系数 | float |
| Label | LabelData | gradient | 文字渐变样式 | 枚举(LabelPartGradientType: 无、Vertical、Horizontal、Diagonal、UpperLeft、UpperRight、LowerLeft、LowerRight) |
| Label | LabelData | height | 高度参数 | float |
| Label | LabelData | horizontalAlignment | 文字水平对齐方式 | 枚举(Left、Center、Right) |
| Label | LabelData | offset | 位置偏移 | Vector3(x,y,z) |
| Label | LabelData | outlineWidth | 文字描边宽度 | float |
| Label | LabelData | paintIndexShift | 涂装索引偏移 | int |
| Label | LabelData | parentPath | 标签父节点路径 | string |
| Label | LabelData | renderQueueOffset | 渲染队列偏移 | int |
| Label | LabelData | supportsCurvature | 是否支持文字弯曲 | bool |
| Label | LabelData | supportsGradient | 是否支持文字渐变 | bool |
| Label | LabelData | verticalAlignment | 文字垂直对齐方式 | 枚举(Top、Middle、Bottom) |
| Label | LabelData | width | 宽度参数 | float |
| Landing Gear | RetractableLandingGearData | （无） | 该零件未在自身State中读取独有属性，主要沿用父类或公共层逻辑 | 无 |
| Landing Gear | WheelData | （无） | 该零件未在自身State中读取独有属性，主要沿用父类或公共层逻辑 | 无 |
| Landing Gear | WingLandingGearData | （无） | 该零件未在自身State中读取独有属性，主要沿用父类或公共层逻辑 | 无 |
| Magnet | MagnetData | activationGroup | 设置功能所属激活组，用于按键触发开关 | string (无、1~8) |
| Magnet | MagnetData | power | 磁力强度/功率 | float |
| Main Rotor | HeliMainRotorData | centerOfMassOffset | 主旋翼系统质心偏移 | Vector3(x,y,z) |
| Main Rotor | HeliMainRotorData | cyclicPitchMaxDeflection | 主旋翼周期俯仰最大偏转角 | float |
| Main Rotor | HeliMainRotorData | cyclicRollMaxDeflection | 主旋翼周期横滚最大偏转角 | float |
| Main Rotor | HeliMainRotorData | rotorDamping | 旋翼振动阻尼系数 | float |
| MFD | MfdData | targetingPod | 关联目标指示吊舱的零件ID | int (目标零件ID) |
| Missile | MissileData | function | 武器用途模式 | 枚举(WeaponFunction: 无、AirToAir、AirToSurface、MultiRole) |
| Missile | MissileData | guidanceActivationDelay | 制导激活延迟 | float |
| Missile | MissileData | ignitionDelay | 点火延迟 | float |
| Missile | MissileData | killCam | 命中后是否启用击杀镜头 | bool |
| Missile | MissileData | loft | 导弹抛物线爬升比例（Loft） | float |
| Missile | MissileData | maxForwardThrustForce | 最大前向推力 | float |
| Missile | MissileData | maxFuelTime | 最大燃烧时间 | float |
| Missile | MissileData | maxHeadingAngleAdjustmentRate | 最大航向修正速率 | float |
| Missile | MissileData | maxRange | 最大作用距离 | float |
| Missile | MissileData | maxSpeed | 最大速度 | float |
| Missile | MissileData | maxTargetingAngle | 最大锁定角 | float |
| Missile | MissileData | maxThrustVectoringRate | 最大推力矢量修正速率 | float |
| Missile | MissileData | maxTorque | 最大扭矩 | float |
| Missile | MissileData | maxVelocityAngleAdjustmentRate | 最大速度矢量修正速率 | float |
| Missile | MissileData | minRange | 最小作用距离 | float |
| Missile | MissileData | proximityDetonationRangeMax | 近炸引信最大触发距离 | float |
| Missile | MissileData | proximityDetonationRangeMin | 近炸引信最小触发距离 | float |
| Missile | MissileData | seeker | 导引头类型 | 枚举(SeekerType: Unguided、Infrared、SemiActiveRadar、ActiveRadar、Laser、AntiRadiation) |
| Missile | MissileData | smokeOpacity | 尾烟不透明度 | float |
| Missile | MissileData | smokeScale | 尾烟缩放 | float |
| Missile | MissileData | waterproof | 是否防水 | bool |
| Missile Configuration | ProceduralMissileData | attachPosition | 导弹在挂点上的前后安装位置 | float (-1~1) |
| Missile Configuration | ProceduralMissileData | body | 程序化导弹机体段样式ID | string |
| Missile Configuration | ProceduralMissileData | burnTime | 发动机燃烧时间比例 | float (0~1) |
| Missile Configuration | ProceduralMissileData | engine | 导弹发动机类型 | 枚举(MissileEngineType: Solid、ThrustVector、Jet) |
| Missile Configuration | ProceduralMissileData | nose | 程序化导弹鼻锥样式ID（可选覆盖） | string |
| Missile Configuration | ProceduralMissileData | noseLength | 导弹头部长度。 | float |
| Missile Configuration | ProceduralMissileData | radius | 半径/作用半径 | float |
| Missile Configuration | ProceduralMissileData | seeker | 导引头/目标搜索参数 | 枚举(SeekerType: Unguided、Infrared、SemiActiveRadar、ActiveRadar、Laser、AntiRadiation) |
| Missile Configuration | ProceduralMissileData | seekerFOV | 导引头/目标搜索参数 | float |
| Missile Configuration | ProceduralMissileData | size | 尺寸/大小 | float |
| Missile Configuration | ProceduralMissileData | updateMissileModifier | 参数变更后刷新导弹修正器。 | bool |
| Missile Configuration | ProceduralMissileData | warheadBias | 战斗部位置偏置参数。 | float |
| Nosecone | AdaptiveNoseConeData | scale | 缩放比例/系数 | Vector3(x,y,z) |
| Parachute | ParachuteData | activationGroup | 激活组索引，用于通过按键或标签控制零件状态 | string |
| Parachute | ParachuteData | size | 尺寸/大小 | float |
| Parachute | ParachuteData | style | 降落伞样式。 | string |
| Part Targeting | PartTargetingData | customPartIds | 自定义目标零件ID列表。 | int列表(逗号分隔) |
| Part Targeting | PartTargetingData | partIds | 引用零件ID列表。 | int列表(逗号分隔) |
| Part Targeting | PartTargetingData | targetMode | 零件目标选择模式。 | 枚举(PartTargetingMode: SinglePart、MultipleParts、Custom) |
| Pedal | PedalData | fullAngle | 全行程角度。 | float |
| Pedal | PedalData | input | 输入源/控制器绑定名称 | string |
| Pedal | PedalData | zeroAngle | 零位角度。 | float |
| Piston | PistonData | attachPoint | 活塞移动端连接点索引。 | int |
| Piston | PistonData | cycle | 是否循环往复运动。 | bool |
| Piston | PistonData | extend | 活塞运动方向（推/拉）。 | bool |
| Piston | PistonData | maxRange | 最大值限制 | float |
| Piston | PistonData | maxSpeed | 最大值限制 | float |
| Piston | PistonData | preventBreaking | 是否启用防断裂保护。 | bool |
| Piston | PistonData | range | 范围/行程/边界值 | float |
| Piston | PistonData | speed | 运动或响应速度 | float |
| Posed Grip | PosedGripData | asButton | 是否按按钮模式处理输入。 | bool |
| Posed Grip | PosedGripData | colliders | 碰撞体路径列表（逗号分隔）。 | string |
| Posed Grip | PosedGripData | control | 控制绑定名称。 | string |
| Posed Grip | PosedGripData | controlPath | XR控制路径。 | string |
| Posed Grip | PosedGripData | disableTooltip | 禁用提示文本显示。 | bool |
| Posed Grip | PosedGripData | gripTarget | 抓地力/摩擦力系数 | string |
| Posed Grip | PosedGripData | gripType | 抓地力/摩擦力系数 | 枚举(XRControlGripType: Default、FlightStick、Throttle) |
| Posed Grip | PosedGripData | outlineScale | 缩放比例/系数 | Vector3(x,y,z) |
| Posed Grip | PosedGripData | pose | 抓握姿态名称。 | string |
| Posed Grip | PosedGripData | previewPose | 编辑器预览姿态。 | string |
| Posed Grip | PosedGripData | processor | 输入处理器表达式。 | string |
| Posed Grip | PosedGripData | tooltip | 提示文本。 | string |
| Posed Grip | PosedGripData | tooltipOffset | 提示偏移值。 | float |
| Posed Grip | PosedGripData | tooltipTransformPath | 提示锚点变换路径。 | string |
| Procedural Bay | ProceduralBayData | doorStyle | 舱门开启样式。 | 枚举(DoorStyle: 无、SingleLeft、SingleRight、Double) |
| Procedural Bay | ProceduralBayData | startOpen | 是否初始为开启状态。 | bool |
| Procedural Window | ProceduralWindowData | hideGlass | 是否隐藏玻璃层。 | bool |
| Propeller Engine | PropEngineAdvancedData | legacyCotPos | 是否使用旧版推力中心位置逻辑。 | bool |
| Propellers | PropellerAssemblyData | bladeBlurCount | 桨叶模糊段数量。 | int |
| Propellers | PropellerAssemblyData | bladeBlurSpread | 桨叶模糊扩散范围。 | float |
| Propellers | PropellerAssemblyData | bladeCount | 桨叶数量。 | int |
| Propellers | PropellerAssemblyData | chordRadiusRatio | 半径/作用半径 | float |
| Propellers | PropellerAssemblyData | chordScale | 缩放比例/系数 | float |
| Propellers | PropellerAssemblyData | defaultDiameter | 默认螺旋桨直径。 | float |
| Propellers | PropellerAssemblyData | density | 密度参数。 | float |
| Propellers | PropellerAssemblyData | dragScalar | 阻力相关参数 | float |
| Propellers | PropellerAssemblyData | hub | 桨毂样式或资源ID。 | string |
| Propellers | PropellerAssemblyData | hubScale | 缩放比例/系数 | float |
| Propellers | PropellerAssemblyData | isWaterProp | 是否为水上螺旋桨。 | bool |
| Propellers | PropellerAssemblyData | magicEngineId | 关联发动机ID。 | int |
| Propellers | PropellerAssemblyData | maxPitch | 最大值限制 | float |
| Propellers | PropellerAssemblyData | pitchControlType | 螺旋桨桨距控制模式。 | 枚举(PropellerAssemblyData.PitchControl: Auto、Fixed、Manual) |
| Propellers | PropellerAssemblyData | propeller | 螺旋桨样式/资源ID。 | string |
| Propellers | PropellerAssemblyData | pushProp | 是否使用推式布局。 | bool |
| Propellers | PropellerAssemblyData | reverseBladeDirection | 是否反转桨叶旋转方向。 | bool |
| Propellers | PropellerAssemblyData | size | 尺寸/大小 | float |
| Propellers | PropellerAssemblyData | thrustScalar | 推力大小 | float |
| Propellers | PropellerAssemblyData | twistAngleRoot | 根部桨叶扭转角。 | float |
| Reaction Control Nozzle | ReactionControlNozzleData | activationGroup | 激活组索引，用于通过按键或标签控制零件状态 | string |
| Reaction Control Nozzle | ReactionControlNozzleData | autoAssignType | 是否自动识别喷口控制轴类型。 | bool |
| Reaction Control Nozzle | ReactionControlNozzleData | fuelConsumptionRate | 燃料消耗速率。 | float |
| Reaction Control Nozzle | ReactionControlNozzleData | power | 功率/强度百分比 | float |
| Reaction Control Nozzle | ReactionControlNozzleData | reverse | 是否反向输出方向。 | bool |
| Reaction Control Nozzle | ReactionControlNozzleData | type | RCS喷口轴向类型（俯仰/横滚/偏航）。 | 枚举(ReactionControlNozzleType: Pitch、Roll、Yaw) |
| Refuel Drouge | RefuelDrogueData | activationGroup | 激活组索引，用于通过按键或标签控制零件状态 | string |
| Refuel Drouge | RefuelDrogueData | angularDragPower | 阻力相关参数 | float |
| Refuel Drouge | RefuelDrogueData | angularStabPower | 角向稳定强度。 | float |
| Refuel Drouge | RefuelDrogueData | transferRate | 传输速率。 | float |
| Refuel Drouge | RefuelDrogueData | triggerColliderPath | 触发碰撞体路径。 | string |
| Refuel Probe | RefuelProbeData | offset | 位置偏移量 | Vector2(x,y) |
| Resizable Shape | ResizableShapeData | attachPointPosition | 空间坐标位置 | Vector3(x,y,z) |
| Resizable Shape | ResizableShapeData | bounciness | 弹性系数。 | float |
| Resizable Shape | ResizableShapeData | friction | 摩擦系数。 | float |
| Resizable Shape | ResizableShapeData | size | 尺寸/大小 | float (runtime radius = value/4) |
| Rocket | RocketWeaponData | activationGroup | 激活组索引，用于通过按键或标签控制零件状态 | string |
| Rocket | RocketWeaponData | burnTimer | 时间参数（时长/周期） | float |
| Rocket | RocketWeaponData | explosionScale | 缩放比例/系数 | float |
| Rocket | RocketWeaponData | finMode | 尾翼模式/配置标记。 | string |
| Rocket | RocketWeaponData | firingDelay | 延迟/滞后时间 | float |
| Rocket | RocketWeaponData | laserGuided | 是否启用激光制导。 | bool |
| Rocket | RocketWeaponData | name | 火箭武器自定义名称。 | string |
| Rocket | RocketWeaponData | selfDestructTimer | 时间参数（时长/周期） | float |
| Rocket Pod | RocketPodData | activationGroup | 激活组索引，用于通过按键或标签控制零件状态 | string |
| Rocket Pod | RocketPodData | explosionScale | 缩放比例/系数 | float |
| Rocket Pod | RocketPodData | firingDelay | 延迟/滞后时间 | float |
| Rocket Pod | RocketPodData | laserGuided | 是否启用激光制导。 | bool |
| Rocket Pod | RocketPodData | name | 火箭吊舱自定义名称。 | string |
| Rotator | JointRotatorData | allowFreeSpin | 是否允许自由旋转。 | bool |
| Rotator | JointRotatorData | attachPoint | 旋转关节连接点索引。 | int |
| Rotator | JointRotatorData | audio | 是否启用旋转音效。 | bool |
| Rotator | JointRotatorData | damperMultiplier | 阻尼倍率。 | float |
| Rotator | JointRotatorData | disableBaseMesh | 是否隐藏基座网格。 | bool |
| Rotator | JointRotatorData | hingeOffset | 铰链偏移量。 | Vector3(x,y,z) |
| Rotator | JointRotatorData | maxRange | 最大值限制 | int |
| Rotator | JointRotatorData | maxSpeed | 最大值限制 | float |
| Rotator | JointRotatorData | minRange | 最小值限制 | int |
| Rotator | JointRotatorData | range | 范围/行程/边界值 | float |
| Rotator | JointRotatorData | shortestAngle | 旋转时是否走最短角度路径。 | bool |
| Rotator | JointRotatorData | speed | 运动或响应速度 | float |
| Rotator | JointRotatorData | supportsDisableBaseMesh | 是否支持隐藏基座网格。 | bool |
| Seat | SeatData | animation | 动画状态/资源名称。 | string |
| Seat | SeatData | exitPosition | 空间坐标位置 | Vector3(x,y,z) |
| Seat | SeatData | exitRotation | 旋转角度/姿态 | Vector3(x,y,z) |
| Seat | SeatData | primarySeat | 是否为主座位。 | bool |
| Seat | SeatData | reclination | 座椅后仰幅度。 | float |
| Seat | SeatData | seatedPosition | 空间坐标位置 | Vector3(x,y,z) |
| Seat | SeatData | seatedRotation | 旋转角度/姿态 | Vector3(x,y,z) |
| Seat IK | IKSeatData | bodyTarget | 身体IK目标。 | int |
| Seat IK | IKSeatData | designerCharacter | 设计器角色ID。 | string |
| Seat IK | IKSeatData | fpvTracking | 是否启用第一人称跟踪。 | bool |
| Seat IK | IKSeatData | leftElbowTarget | 左肘IK目标。 | int |
| Seat IK | IKSeatData | leftFootTarget | 左脚IK目标。 | int |
| Seat IK | IKSeatData | leftHandTarget | 左手IK目标。 | int |
| Seat IK | IKSeatData | leftKneeTarget | 左膝IK目标。 | int |
| Seat IK | IKSeatData | leftShoulderTarget | 左肩IK目标。 | int |
| Seat IK | IKSeatData | maintainHeadRotation | 旋转角度/姿态 | float |
| Seat IK | IKSeatData | rightElbowTarget | 右肘IK目标。 | int |
| Seat IK | IKSeatData | rightFootTarget | 右脚IK目标。 | int |
| Seat IK | IKSeatData | rightHandTarget | 右手IK目标。 | int |
| Seat IK | IKSeatData | rightKneeTarget | 右膝IK目标。 | int |
| Seat IK | IKSeatData | rightShoulderTarget | 右肩IK目标。 | int |
| Seat IK | IKSeatData | selfAssignTargets | 是否自动分配IK目标。 | bool |
| Seat IK | IKSeatData | snapRange | IK吸附范围。 | float |
| Suspension | SuspensionData | attachPoint | 悬挂连接点索引。 | int |
| Suspension | SuspensionData | damper | 阻尼系数。 | float |
| Suspension | SuspensionData | spring | 弹簧刚度。 | float |
| Switch | CockpitSwitchData | angleOff | 关闭状态角度。 | float |
| Switch | CockpitSwitchData | angleOn | 开启状态角度。 | float |
| Switch | CockpitSwitchData | axis | 轴向映射。 | Vector3(x,y,z) |
| Switch | CockpitSwitchData | disableTooltip | 禁用提示文本显示。 | bool |
| Switch | CockpitSwitchData | inputId | 输入标识符。 | string |
| Switch | CockpitSwitchData | outputValue | 输出值。 | float |
| Switch | CockpitSwitchData | positionTransitionDelay | 延迟/滞后时间 | float |
| Switch | CockpitSwitchData | positionTransitionTime | 时间参数（时长/周期） | float |
| Switch | CockpitSwitchData | scale | 缩放比例/系数 | float |
| Switch | CockpitSwitchData | style | 驾驶舱开关样式。 | 枚举(CockpitSwitchData.CockpitSwitchStyle: Default、Flip、Rocker、Pivot) |
| Switch | CockpitSwitchData | tooltip | 提示文本。 | string |
| Tail Rotor | HeliTailRotorData | linkageSpeed | 联动响应速度。 | float |
| Tail Rotor | HeliTailRotorData | pidGainsHeadingHold | 航向保持PID增益。 | Vector3(x,y,z) |
| Tail Rotor | HeliTailRotorData | pidGainsRate | 速率控制PID增益。 | Vector3(x,y,z) |
| Tail Rotor | HeliTailRotorData | tailMode | 尾桨模式。 | 枚举(HeliTailRotorData.TailModeType: HeadingHold、Rate、Manual) |
| Tail Rotor | HeliTailRotorData | tailSpeed | 尾桨响应速度。 | float |
| Tail Rotor | HeliTailRotorData | trimScale | 缩放比例/系数 | float |
| Targeting Pod | TargetingPodData | activationGroup | 激活组索引，用于通过按键或标签控制零件状态 | string |
| Targeting Pod | TargetingPodData | defaultActivationGroup | 默认激活组，零件初始化所属的激活组 | string |
| Targeting Pod | TargetingPodData | maxDistance | 最大作用距离 | float |
| Targeting Pod | TargetingPodData | offset | 位置偏移量 | Vector3(x,y,z) |
| Text Decal | TextDecalData | alignH | 文本水平对齐方式。 | 枚举(TextDecalData.HorizontalTextAlignment: Center、Left、Right、Stretch) |
| Text Decal | TextDecalData | alignV | 文本垂直对齐方式。 | 枚举(TextDecalData.VerticalTextAlignment: Center、Top、Bottom) |
| Text Decal | TextDecalData | font | 字体样式。 | 枚举(TextDecalData.FontStyle: Default、Roboto、Military、FourteenSegment、Stencil) |
| Text Decal | TextDecalData | fontSize | 尺寸/大小 | float |
| Text Decal | TextDecalData | text | 显示文本。 | string |
| Thrust Port | EngineThrustPortData | exhaustScale | 缩放比例/系数 | Vector3(x,y,z) |
| Torpedo | TorpedoData | （无） | 该零件未在自身 State 中读取独有属性，主要沿用父类或公共层逻辑 | 无 |
| Transmission | JTransmissionData | customGearRatios | 自定义档位传动比列表。 | float列表(逗号分隔) |
| Transmission | JTransmissionData | finalGearRatio | 最终传动比。 | float |
| Transmission | JTransmissionData | gearProfile | 档位预设曲线。 | 枚举(JTransmissionData.JGearProfileType: Street、Racing、Offroad、Custom) |
| Transmission | JTransmissionData | gearTuning | 档位调校系数。 | float |
| Transmission | JTransmissionData | numGears | 档位数量。 | int |
| Transmission | JTransmissionData | postShiftBan | 换挡后锁止持续时间。 | float |
| Transmission | JTransmissionData | reverseGearRatio | 倒档传动比。 | float |
| Transmission | JTransmissionData | shiftDownRpm | 降档转速阈值。 | float |
| Transmission | JTransmissionData | shiftDuration | 换挡持续时间。 | float |
| Transmission | JTransmissionData | shiftGuardSpeedThreshold | 换挡保护速度阈值。 | float |
| Transmission | JTransmissionData | shiftUpRpm | 升档转速阈值。 | float |
| Transmission | JTransmissionData | size | 尺寸/大小 | float |
| Transmission | JTransmissionData | transmissionType | 变速箱类型。 | 枚举(JTransmissionData.JTransmissionType: Automatic、Manual) |
| Transmission | JTransmissionData | variableShift | 可变换挡策略参数。 | float |
| Transparency | TransparencyData | alwaysFindConnected | 计算透明度时始终包含已连接零件。 | bool |
| Transparency | TransparencyData | hideBack | 是否隐藏背面。 | bool |
| Transparency | TransparencyData | hideFront | 是否隐藏正面。 | bool |
| Transparency | TransparencyData | hideInside | 是否隐藏内部面。 | bool |
| Transparency | TransparencyData | opacity | 不透明度值。 | float |
| Transparency | TransparencyData | overrideHide | 是否覆盖默认隐藏行为。 | bool |
| Wheel | JWheelData | brake | 制动力度。 | float |
| Wheel | JWheelData | duals | 是否双轮胎配置。 | bool |
| Wheel | JWheelData | forcePoint | 受力点参数。 | float |
| Wheel | JWheelData | frictionCirclePower | 摩擦圆功率参数。 | float |
| Wheel | JWheelData | frictionCircleStrength | 摩擦圆强度参数。 | float |
| Wheel | JWheelData | frictionPreset | 摩擦预设ID/名称。 | string |
| Wheel | JWheelData | hideRims | 是否隐藏轮圈。 | bool |
| Wheel | JWheelData | magicEngineId | 关联发动机ID。 | int |
| Wheel | JWheelData | reversed | 是否反转车轮方向。 | bool |
| Wheel | JWheelData | rim | 轮圈样式。 | string |
| Wheel | JWheelData | rimOffset | 轮圈偏移。 | float |
| Wheel | JWheelData | size | 尺寸/大小 | float |
| Wheel | JWheelData | tire | 轮胎样式。 | string |
| Wheel | JWheelData | tractionForward | 前向抓地力系数。 | float |
| Wheel | JWheelData | tractionSideways | 侧向抓地力系数。 | float |
| Wheel | JWheelData | turningAngle | 最大转向角。 | float |
| Wheel | JWheelData | turningAngleDampening | 转向角阻尼。 | float |
| Wheel | JWheelData | turningRate | 转向速率。 | float |
| Wheel | JWheelData | width | 车轮宽度系数。 | float |
| Wheel | ResizableWheelData | brakeTorque | 扭矩/转矩 | float |
| Wheel | ResizableWheelData | damper | 阻尼系数。 | float |
| Wheel | ResizableWheelData | direction | 驱动/旋转方向。 | string |
| Wheel | ResizableWheelData | enableAutoTraction | 是否启用自动牵引控制。 | bool |
| Wheel | ResizableWheelData | enableSuspension | 悬挂系统调节 | bool |
| Wheel | ResizableWheelData | engineId | 发动机ID。 | int |
| Wheel | ResizableWheelData | hideRims | 是否隐藏轮圈。 | bool |
| Wheel | ResizableWheelData | maxAngularVelocity | 最大值限制 | float |
| Wheel | ResizableWheelData | size | 尺寸/大小 | float |
| Wheel | ResizableWheelData | slipForwardAsymptote | 前向滑移渐近值。 | float |
| Wheel | ResizableWheelData | slipForwardExtremum | 前向滑移极值。 | float |
| Wheel | ResizableWheelData | slipSidewaysAsymptote | 侧向滑移渐近值。 | float |
| Wheel | ResizableWheelData | slipSidewaysExtremum | 侧向滑移极值。 | float |
| Wheel | ResizableWheelData | spring | 弹簧刚度。 | float |
| Wheel | ResizableWheelData | tire | 轮胎样式。 | string |
| Wheel | ResizableWheelData | tractionForward | 前向抓地力系数。 | float |
| Wheel | ResizableWheelData | tractionSideways | 侧向抓地力系数。 | float |
| Wheel | ResizableWheelData | turningAngle | 最大转向角。 | float |
| Wheel | ResizableWheelData | turningRate | 转向速率。 | float |
| Wheel | ResizableWheelData | width | 车轮宽度系数。 | float |
| Wheel Suspension | JWheelSuspensionData | damper | 阻尼系数。 | float |
| Wheel Suspension | JWheelSuspensionData | extension | 悬挂行程。 | float |
| Wheel Suspension | JWheelSuspensionData | rideHeight | 离地高度。 | float |
| Wheel Suspension | JWheelSuspensionData | shockPosition | 空间坐标位置 | float |
| Wheel Suspension | JWheelSuspensionData | size | 尺寸/大小 | float |
| Wheel Suspension | JWheelSuspensionData | stiffness | 刚度系数。 | float |
| Wheel Suspension | JWheelSuspensionData | suspensionLength | 悬挂系统调节 | float |
| Winch | WinchData | attachPoint | 绞盘缆绳连接点索引。 | int |
| Winch | WinchData | breakScale | 缩放比例/系数 | float |
| Winch | WinchData | range | 范围/行程/边界值 | float |
| Winch | WinchData | speed | 运动或响应速度 | float |
| Winch | WinchData | startRange | 初始缆绳长度/范围值。 | float |
| Winch | WinchData | volume | 音量参数。 | float |
| Wing | JWingData | axis | 轴向映射。 | string |
| Wing | JWingData | chordSamples | 弦长采样数量。 | int |
| Wing | JWingData | colliderSamples | 碰撞体采样数量。 | int |
| Wing | JWingData | disableWingtipVortices | 是否禁用翼尖涡流。 | bool |
| Wing | JWingData | flipped | 是否翻转翼型方向。 | bool |
| Wing | JWingData | fuelFraction | 燃料比例。 | float |
| Wing | JWingData | invert | 是否反向输出/取反 | bool |
| Wing | JWingData | invertOnMirror | 镜像零件时是否反向。 | bool |
| Wing | JWingData | liftScale | 缩放比例/系数 | float |
| Wing | JWingData | partIds | 引用零件ID列表。 | string |
| Wing | JWingData | style | 机翼样式兼容字段（主要用于迁移/旧版数据）。 | string (legacy compatible style marker) |
| Wing | JWingData | version | 序列化数据版本。 | int |
| Wing | JWingData | viscousDragScale | 缩放比例/系数 | float |
| Wing | JWingData | zeroLiftDragScale | 缩放比例/系数 | float |
| Wing | WingData | airfoil | 翼型类型。 | string |
| Wing | WingData | allowControlSurfaces | 是否允许舵面控制。 | bool |
| Wing | WingData | angleOfAttack | 攻角参数。 | float |
| Wing | WingData | baseThickness | 根部厚度。 | float |
| Wing | WingData | density | 密度参数。 | float |
| Wing | WingData | fuelPercentage | 燃料百分比。 | float |
| Wing | WingData | hingeDistance | 铰链距离。 | float |
| Wing | WingData | inverted | 是否倒置标记。 | bool |
| Wing | WingData | liftScale | 缩放比例/系数 | float |
| Wing | WingData | minSectionLength | 最小值限制 | float |
| Wing | WingData | rootLeadingOffset | 根部前缘偏移。 | float |
| Wing | WingData | rootTrailingOffset | 根部后缘偏移。 | float |
| Wing | WingData | tipLeadingOffset | 翼尖前缘偏移。 | float |
| Wing | WingData | tipPosition | 空间坐标位置 | Vector3(x,y,z) |
| Wing | WingData | tipThickness | 翼尖厚度。 | float |
| Wing | WingData | tipTrailingOffset | 翼尖后缘偏移。 | float |
