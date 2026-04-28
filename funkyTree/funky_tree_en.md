## Funky Tree Parameter List

### Unit Conventions (Based on Source Code)

- Angle-related values: unit is **degrees (°)**.
- Angular-rate-related values: unit is **degrees per second (°/s)**.
- Time-related values: unit is **seconds (s)**
- Distance / altitude / coordinate-related values: use game world coordinate units (Unity world unit, typically interpreted as meters in this project).
- Speed-related values: world coordinate units per second (typically interpreted as **m/s**).
- In this project, `Latitude`/`Longitude` are axis coordinates (`z/x`), **not geographic latitude/longitude degrees, game units are typically interpreted as meters**.

### Constants

| Category | Parameter Name | Description | Return Type/Content |
|---|---|---|---|
| Constant | `true` | Boolean true constant | `bool` |
| Constant | `false` | Boolean false constant | `bool` |
| Constant | `pi` | Pi constant | `number(float)` |
| Constant | `e` | Current implementation is `Mathf.Log(1f)`, value is `0` (note: not the common mathematical $e\approx2.718$) | `number(float)` |

### Default Functions (Built-in)

| Category | Parameter Name | Description | Return Type/Content |
|---|---|---|---|
| Default Function | `abs(x)` | Absolute value, `x:number` | `number(float)` |
| Default Function | `acos(x)` | Arccosine. Input `x:number` (unitless, common range `[-1,1]`), **returns degrees (°)** | `number(float)` |
| Default Function | `asin(x)` | Arcsine. Input `x:number` (unitless, common range `[-1,1]`), **returns degrees (°)** | `number(float)` |
| Default Function | `atan(x)` | Arctangent. Input `x:number` (unitless), **returns degrees (°)** | `number(float)` |
| Default Function | `atan2(y, x)` | Two-argument arctangent. `y:number, x:number` (same dimension), **returns degrees (°)** | `number(float)` |
| Default Function | `ceil(x)` | Round up. `x:number`; return type is still `float`, but value is integer-like | `number(float)` |
| Default Function | `clamp(value, min, max)` | Clamp value. All three params are `number` | `number(float)` |
| Default Function | `clamp01(value)` | Clamp to `[0,1]`, `value:number` | `number(float)` |
| Default Function | `cos(angle)` | Cosine. Input `angle:number` (unit **°**) | `number(float)` |
| Default Function | `deltaangle(current, target)` | Shortest angular difference. `current:number, target:number` (angles, unit **°**); returns angular delta roughly in `[-180, 180]` | `number(float)` |
| Default Function | `exp(x)` | Natural exponential function, computes $e^x$ (this $e$ is the mathematical constant and does not depend on the context constant `e`) | `number(float)` |
| Default Function | `floor(x)` | Round down. `x:number`; return type is still `float`, but value is integer-like | `number(float)` |
| Default Function | `format(value, format)` | Numeric formatting. `value:number, format:string`. If the first format letter is `D/d/X/x`, source casts `value` to `int` first | `string` |
| Default Function | `inverselerp(a, b, value)` | Inverse lerp. `a,b,value:number`; returns interpolation factor `t` (`Mathf.InverseLerp`, clamped to `[0,1]`) | `number(float)` |
| Default Function | `lerp(a, b, t)` | Linear interpolation. `a,b,t:number`; in implementation, `t` is clamped to `[0,1]` | `number(float)` |
| Default Function | `lerpangle(a, b, t)` | Angle interpolation. `a,b` are angles (unit **°**), `t` is unitless interpolation factor | `number(float)` |
| Default Function | `lerpunclamped(a, b, t)` | Unclamped linear interpolation. All three params are `number` | `number(float)` |
| Default Function | `log(value, base)` | Logarithm, `value:number, base:number` (maps to `Mathf.Log(value, base)`) | `number(float)` |
| Default Function | `log10(x)` | Base-10 logarithm, `x:number` | `number(float)` |
| Default Function | `max(a, b)` | Maximum value, `a:number, b:number` | `number(float)` |
| Default Function | `min(a, b)` | Minimum value, `a:number, b:number` | `number(float)` |
| Default Function | `pingpong(t, length)` | Ping-pong oscillation. `t:number, length:number`; returns within `[0, length]` | `number(float)` |
| Default Function | `pow(value, power)` | Power operation, `value:number, power:number` | `number(float)` |
| Default Function | `repeat(t, length)` | Periodic repeat. `t:number, length:number`; returns in `[0, length)` (`Mathf.Repeat`) | `number(float)` |
| Default Function | `round(x)` | Round to nearest integer, `x:number`; return type is still `float` | `number(float)` |
| Default Function | `sign(x)` | Sign function, `x:number`; maps to `Mathf.Sign`, returns `1` for `x >= 0`, `-1` for `x < 0` | `number(float)` |
| Default Function | `sin(angle)` | Sine. Input `angle:number` (unit **°**) | `number(float)` |
| Default Function | `smoothstep(from, to, t)` | Smooth interpolation. `from,to,t:number`; implementation clamps `t` to `[0,1]` first | `number(float)` |
| Default Function | `sqrt(x)` | Square root, `x:number` | `number(float)` |
| Default Function | `tan(angle)` | Tangent. Input `angle:number` (unit **°**) | `number(float)` |

### Special Functions (Stateful)

| Category | Parameter Name | Description | Return Type/Content |
|---|---|---|---|
| Special Function | `sum(value)` | Integrator. `value:number`, accumulated each frame by $\Delta t$ (seconds): $S\leftarrow S+value\cdot\Delta t$. If `value` unit is `U`, result unit is `U·s` | `number(float)` |
| Special Function | `rate(value)` | Differentiator. `value:number`, computes rate of change: $\frac{value-last}{\Delta t}$. If `value` unit is `U`, result unit is `U/s`; first call returns `0` | `number(float)` |
| Special Function | `PID(target, current, p, i, d)` | PID output. Source logic: `error = target - current`, `I += error*dt`, `D = (lastCurrent - current)/dt` (first time is 0), output `p*error + i*I + d*D` | `number(float)` |
| Special Function | `smooth(value, maxRate)` | Rate-limited smoothing. Source is based on `MoveTowards(last, value, maxRate*dt)`, first call directly returns current `value` | `number(float)` |

### Flight State Exposure (`[Exposed]` in `AircraftScript`)

| Category | Parameter Name | Description | Return Type/Content |
|---|---|---|---|
| Flight State Property | `Altitude` | Altitude (relative to sea level), from `GlobalPosition.y - SeaLevel` (world distance unit, typically meters) | `number(float)` |
| Flight State Property | `AltitudeAgl` | Height above ground (AGL), from raycast distance `RaycastHit.distance` (world distance unit, typically meters) | `number(float)` |
| Flight State Property | `Rpm1` | Engine/channel 1 RPM (revolutions per minute) | `number(float)` |
| Flight State Property | `Rpm2` | Engine/channel 2 RPM (revolutions per minute) | `number(float)` |
| Flight State Property | `Rpm3` | Engine/channel 3 RPM (revolutions per minute) | `number(float)` |
| Flight State Property | `Rpm4` | Engine/channel 4 RPM (revolutions per minute) | `number(float)` |
| Flight State Property | `AngleOfAttack` | Angle of attack (AoA, unit **°**) | `number(float)` |
| Flight State Property | `AngleOfSlip` | Sideslip angle (unit **°**) | `number(float)` |
| Flight State Property | `Fuel` | Fuel proportion (source alias mapped from `FuelProportion`) | `number(float)` |
| Flight State Property | `GForce` | Total G-force (unit **g**, 1g≈9.81m/s²) | `number(float)` |
| Flight State Property | `GS` | Ground speed (world speed unit, typically m/s) | `number(float)` |
| Flight State Property | `Heading` | Heading angle (unit **°**) | `number(float)` |
| Flight State Property | `IAS` | Indicated airspeed (world speed unit, typically m/s) | `number(float)` |
| Flight State Property | `Latitude` | Actually `GlobalPosition.z` coordinate value (world unit, **not geographic latitude degrees**) | `number(float)` |
| Flight State Property | `Longitude` | Actually `GlobalPosition.x` coordinate value (world unit, **not geographic longitude degrees**) | `number(float)` |
| Flight State Property | `PitchAngle` | Pitch angle (unit **°**) | `number(float)` |
| Flight State Property | `PitchRate` | Pitch angular rate (unit **°/s**) | `number(float)` |
| Flight State Property | `RollAngle` | Roll angle (unit **°**) | `number(float)` |
| Flight State Property | `RollRate` | Roll angular rate (unit **°/s**) | `number(float)` |
| Flight State Property | `SelectedWeapon` | Current selected weapon name (alias mapped from `SelectedWeaponName`) | `string` |
| Flight State Property | `TargetDistance` | Target distance (world distance unit, typically meters) | `number(float)` |
| Flight State Property | `TargetElevation` | Target elevation angle (unit **°**) | `number(float)` |
| Flight State Property | `TargetHeading` | Target heading/bearing angle (unit **°**) | `number(float)` |
| Flight State Property | `TargetLocked` | Whether target is locked | `bool` |
| Flight State Property | `TargetLocking` | Whether target lock is in progress | `bool` |
| Flight State Property | `TargetSelected` | Whether a target is currently selected | `bool` |
| Flight State Property | `TAS` | True airspeed (world speed unit, typically m/s) | `number(float)` |
| Flight State Property | `Time` | Flight time (alias mapped from `TimeSinceStart`, unit **s**) | `number(float)` |
| Flight State Property | `VerticalG` | Vertical G-force (unit **g**) | `number(float)` |
| Flight State Property | `YawRate` | Yaw angular rate (unit **°/s**) | `number(float)` |
| Flight State Method | `ammo(weapon)` | Query weapon ammo. Input: `weapon:string` (weapon name); returns current ammo count for that weapon | `number(float)` |

### Control Inputs / Context Variables (`AircraftControls.SetupContext` + local control-surface vars)

| Category | Parameter Name | Description | Return Type/Content |
|---|---|---|---|
| Control Input Variable | `Trim` | Trim input | `number(float)` |
| Control Input Variable | `Flaps` | Flaps input | `number(float)` |
| Control Input Variable | `Vtol` | VTOL transition input | `number(float)` |
| Control Input Variable | `Roll` | Roll input | `number(float)` |
| Control Input Variable | `Pitch` | Pitch input | `number(float)` |
| Control Input Variable | `Yaw` | Yaw input | `number(float)` |
| Control Input Variable | `Brake` | Brake input | `number(float)` |
| Control Input Variable | `Throttle` | Throttle input | `number(float)` |
| Control Input Variable | `GearDown` | Whether landing gear is down | `bool` |
| Control Input Variable | `LandingGear` | Legacy landing gear float value (down=0, up=1) | `number(float)` |
| Control Input Variable | `FireGuns` | Guns fire input | `bool` |
| Control Input Variable | `FireWeapons` | Weapon launch/fire input | `bool` |
| Control Input Variable | `LaunchCountermeasures` | Countermeasure release input | `bool` |
| Control Input Variable | `ParkingBrake` | Parking brake state | `bool` |
| Control Input Variable | `Activate1` | Activation group 1 state | `bool` |
| Control Input Variable | `Activate2` | Activation group 2 state | `bool` |
| Control Input Variable | `Activate3` | Activation group 3 state | `bool` |
| Control Input Variable | `Activate4` | Activation group 4 state | `bool` |
| Control Input Variable | `Activate5` | Activation group 5 state | `bool` |
| Control Input Variable | `Activate6` | Activation group 6 state | `bool` |
| Control Input Variable | `Activate7` | Activation group 7 state | `bool` |
| Control Input Variable | `Activate8` | Activation group 8 state | `bool` |
| Local Control Surface Variable | `Aileron` | Local aileron value (accounts for wing flip direction) | `number(float)` |
| Local Control Surface Variable | `WingFlipped` | Wing flip direction flag (`-1` or `1`) | `number(float)` |

### Event/Signal Parameters (`VariableOutput` + dynamic declarations)

| Category | Parameter Name | Description | Return Type/Content | Applicable Part (Source Script) |
|---|---|---|---|---|
| Event/Signal | `Altitude` | Altitude output signal (world height unit, typically meters) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal | `Ammo` | Ammo remaining output (e.g., countermeasure dispenser) | `number(float)` | `CounterMeasureDispenserScript` (Countermeasure Dispenser) |
| Event/Signal | `Current Angle` | Current angle output (joint/rotating part, unit **°**) | `number(float)` | `JointRotatorScript` (Joint Rotator) |
| Event/Signal | `Drag Force` | Drag force magnitude output | `number(float)` | `WingScript` (Wing) |
| Event/Signal | `Extension` | Suspension/shock extension amount | `number(float)` | `SuspensionScript` (Suspension) |
| Event/Signal | `Fired` | Fire trigger signal (missile/bomb, often represented as `0/1` pulse) | `number(float)` | `BombScript` (Bomb), `MissileScript` (Missile) |
| Event/Signal | `Forward Slip` | Forward slip amount (wheel/tire) | `number(float)` | `ResizableWheelScript` (Resizable Wheel), `Car/JWheelScript` (Vehicle Wheel) |
| Event/Signal | `Gear` | Current gear | `number(float)` | `Powertrain/JTransmissionScript` (Powertrain Transmission) |
| Event/Signal | `GearRatio` | Current gear ratio | `number(float)` | `Powertrain/JTransmissionScript` (Powertrain Transmission) |
| Event/Signal | `Heading Angle` | Heading angle output (unit **°**) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal | `InputTorque` | Input torque | `number(float)` | `Powertrain/JTransmissionScript` (Powertrain Transmission) |
| Event/Signal | `Is Active` | Active-state signal (camera vantage etc.; source emits `0f/1f`) | `number(float)` | `CameraVantageScript` (Camera Vantage) |
| Event/Signal | `Latitude` | Actually position `z` coordinate output (world unit, **not geographic latitude degrees**) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal | `Lift Force` | Lift force magnitude output | `number(float)` | `WingScript` (Wing) |
| Event/Signal | `Longitude` | Actually position `x` coordinate output (world unit, **not geographic longitude degrees**) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal | `Look Pitch` | View pitch output (unit **°**) | `number(float)` | `CameraVantageScript` (Camera Vantage) |
| Event/Signal | `Look Roll` | View roll output (unit **°**) | `number(float)` | `CameraVantageScript` (Camera Vantage) |
| Event/Signal | `Look Yaw` | View yaw output (unit **°**) | `number(float)` | `CameraVantageScript` (Camera Vantage) |
| Event/Signal | `Offroad` | Offroad/off-surface state amount | `number(float)` | `ResizableWheelScript` (Resizable Wheel), `Car/JWheelScript` (Vehicle Wheel) |
| Event/Signal | `OutputTorque` | Output torque | `number(float)` | `Powertrain/JEngineScript` (Powertrain Engine), `Powertrain/JTransmissionScript` (Powertrain Transmission) |
| Event/Signal | `Pitch Angle` | Pitch angle output (unit **°**) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal | `Pitch Rate` | Pitch angular-rate output (unit **°/s**) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal | `Roll Angle` | Roll angle output (unit **°**) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal | `Roll Rate` | Roll angular-rate output (unit **°/s**) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal | `RPM` | RPM output (revolutions per minute) | `number(float)` | `BladedEngineScript` (Bladed Engine), `CarEngineScript` (Car Engine), `HeliMainRotorScript` (Helicopter Main Rotor), `ResizableWheelScript` (Resizable Wheel), `Car/JWheelScript` (Vehicle Wheel), `Powertrain/JEngineScript` (Powertrain Engine) |
| Event/Signal | `Sideways Slip` | Side slip amount (wheel/tire) | `number(float)` | `ResizableWheelScript` (Resizable Wheel), `Car/JWheelScript` (Vehicle Wheel) |
| Event/Signal | `Speed` | Speed output (world speed unit, typically m/s) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal | `Thrust` | Thrust output | `number(float)` | `EngineScript` (Engine base class) and its derived engine parts |
| Event/Signal | `View Offset X` | View offset X (position offset, world/local unit, typically meters) | `number(float)` | `CameraVantageScript` (Camera Vantage) |
| Event/Signal | `View Offset Y` | View offset Y (position offset, world/local unit, typically meters) | `number(float)` | `CameraVantageScript` (Camera Vantage) |
| Event/Signal | `View Offset Z` | View offset Z (position offset, world/local unit, typically meters) | `number(float)` | `CameraVantageScript` (Camera Vantage) |
| Event/Signal | `Yaw Rate` | Yaw angular-rate output (unit **°/s**) | `number(float)` | `CockpitScript` (Cockpit) |
| Event/Signal (Dynamic Declaration) | `<custom variable name>` (`<自定义变量名>`) | Non-fixed label: variable name comes from part configuration (usually input ID; if it contains `:`, only prefix is used). Therefore it does not appear in fixed `[VariableOutput]` lists | `number(float)` | `CockpitButtonScript` (Cockpit Button), `CockpitSwitchScript` (Cockpit Switch) |
| Event/Signal (Dynamic Declaration) | `<axis variable name>` (`<轴变量名>`) | Non-fixed label: comes from XR control-axis `Variable.Name` (dynamically determined by `ControlBase` axis configuration) | `number(float)` | `XR/ControlBaseScript` (XR Control Base) |
