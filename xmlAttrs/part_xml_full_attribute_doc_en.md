## Part XML Attribute Documentation
- Total part types: 83
- Total attribute rows: 654
- Parts without unique attributes: 5

## Note:
- This document is generated from AI-assisted extraction and may contain inaccuracies in field descriptions.
- Boolean values are represented as true/false.
- For enum types, the value in XML should be a string that matches the case and format of the original enum object. For example, if the document lists an enum as "Enum(CannonData.ProjectileStyle: Sphere, Slug)", then in the XML it should be written as "Sphere" or "Slug", not in lowercase or any other variation.

## Attribute List

| Part Category | Part Class | Attribute | Description | Input Type |
| --- | --- | --- | --- | --- |
| Advanced Performance Scalars | RotorPerfScalarsData | collectiveDrag | Drag scaling coefficient corresponding to main rotor collective pitch. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | collectiveLift | Lift scaling coefficient corresponding to main rotor collective pitch. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | collectiveTorque | Torque scaling coefficient corresponding to main rotor collective pitch. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicMotorDragTorque | Motor resistance torque scaling due to cyclic manipulation. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicPitchInputExpo | Periodic pitch input exponential curve. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicRollInputExpo | Periodic roll input exponential curve. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicRpmFalloffExpo | Exponential curve of cycle control decaying with rotational speed. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicStrength | Overall intensity coefficient of cycle manipulation. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | groundEffect | Ground effect gain factor. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | gyroscopicLag | Rotor gyro response lag coefficient. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | gyroscopicStabilization | Rotor gyro stability coefficient. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | relativeWindPassiveLift | Relative wind passive lift coefficient. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | relativeWindPassiveTorque | Relative wind passive torque coefficient. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | relativeWindPeakSpeed | Relative wind effect peak speed. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | rotorTensor | Rotor moment of inertia coefficient. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | translationalLift | Translational lift coefficient. | float |
| Airbrake | AirBrakeData | drag | Air brake drag coefficient. | float |
| Arresting Hook | ArrestingHookData | activationGroup | Activation group used for grouped key/control triggering. | string (1~8) |
| Arresting Hook | ArrestingHookData | cableDeceleration | Deceleration coefficient applied by the arresting cable to the aircraft. | float |
| Arresting Hook | ArrestingHookData | deployedAngle | Arresting hook lowering angle (degrees). | float |
| Attitude Ball | AttitudeBallData | meshPath | Target mesh path. | string |
| Attitude Ball | AttitudeBallData | rotationType | Attitude ball rotation mode (rotate using selected axis combination). | Enum(AttitudeBallData.BallType: None, Roll, Pitch, Heading, Attitude, LevelCompass, AllAxis) |
| Attitude Ball | AttitudeBallData | scale | Scale factor. | float |
| Beacon Light | BeaconLightData | activationGroup | Activation group used for grouped key/control triggering. | int (0~8,0=All) |
| Beacon Light | BeaconLightData | blinkProgram | Beacon light flashing sequence (duration of each segment, unit seconds, separated by commas). | float list (comma separated seconds) |
| Beacon Light | BeaconLightData | designerBlinkProgram | Blink preset styles used by the designer. | Enum(Preset: Steady, Slow Blink, Quick Blink) |
| Beacon Light | BeaconLightData | input | Input axis/button ID. | string |
| Beacon Light | BeaconLightData | intensity | Effect strength. | float |
| Beacon Light | BeaconLightData | showHalo | Whether to display the beacon light halo effect. | bool |
| Bomb | BombData | (none) | This part reads no unique attribute in its own state; behavior mainly comes from base/shared logic. | None |
| Button | CockpitButtonData | depthBase | Button base depth. | float |
| Button | CockpitButtonData | depthOff | Depth when button is not pressed. | float |
| Button | CockpitButtonData | depthOn | Depth when button pressed. | float |
| Button | CockpitButtonData | disableTooltip | Whether to disable button prompt text. | bool |
| Button | CockpitButtonData | height | Control height. | float |
| Button | CockpitButtonData | inputId | Button binding input ID. | string |
| Button | CockpitButtonData | lightStrength | Button light intensity. | float |
| Button | CockpitButtonData | lightTransitionDelay | Button light change delay. | float |
| Button | CockpitButtonData | lightTransitionTime | Button light change duration. | float |
| Button | CockpitButtonData | outputValue | Button output value. | float |
| Button | CockpitButtonData | padding | Button padding. | float |
| Button | CockpitButtonData | positionTransitionDelay | Button position animation delay. | float |
| Button | CockpitButtonData | positionTransitionTime | Button position animation duration. | float |
| Button | CockpitButtonData | style | Button appearance style. | Enum(CockpitButtonStyle: Rectangular, Circular) |
| Button | CockpitButtonData | tooltip | Button prompt text. | string |
| Button | CockpitButtonData | width | Width. | float |
| Cannon | CannonData | activationGroup | Activation group used for grouped key/control triggering. | string (0/1~8,0=All) |
| Cannon | CannonData | ammoCount | Total number of cannon ammunition. | int |
| Cannon | CannonData | barrelLength | Barrel length. | float |
| Cannon | CannonData | barrelRecoil | Barrel recoil stroke coefficient. | float |
| Cannon | CannonData | baseLength | Mount length. | float |
| Cannon | CannonData | diameter | Cannon caliber/diameter. | float |
| Cannon | CannonData | explosionScalar | Explosion damage multiplier. | float |
| Cannon | CannonData | firingDelay | Minimum gun firing interval. | float |
| Cannon | CannonData | flashScale | Muzzle flash scale. | float |
| Cannon | CannonData | flashSpace | Muzzle flash particle simulation space. | Enum(ParticleSystemSimulationSpace: Local, World, Custom；Customfalls back to Local) |
| Cannon | CannonData | function | Weapon usage mode (air-to-air / air-to-surface / multirole). | Enum(WeaponFunction: None, AirToAir, AirToSurface, MultiRole) |
| Cannon | CannonData | fuseInput | Fuze trigger expression. | string |
| Cannon | CannonData | impactDamageScalar | Impact hit damage multiplier. | float |
| Cannon | CannonData | launchVolume | Launch sound volume. | float |
| Cannon | CannonData | muzzleBrake | Whether to enable muzzle brake. | bool |
| Cannon | CannonData | name | Custom name. | string |
| Cannon | CannonData | projectileLifetime | Projectile lifetime (seconds). | float |
| Cannon | CannonData | projectileStyle | Projectile geometry. | Enum(CannonData.ProjectileStyle: Sphere, Slug) |
| Cannon | CannonData | projectileType | Projectile damage type. | Enum(CannonData.ProjectileType: Basic, Explosive) |
| Cannon | CannonData | projectileVelocity | Projectile initial velocity. | float |
| Cannon | CannonData | recoilForce | Recoil coefficient. | float |
| Cannon | CannonData | tracerColor | Tracer color. | Color(HTML Hex #RRGGBB/#RRGGBBAA) |
| Cannon | CannonData | tracerLength | Tracer length. | float |
| Cannon | CannonData | tracerSpacing | Tracer interval (every N shots). | int |
| Canopy | CanopyData | activationGroup | Activation group used for grouped key/control triggering. | int (0~8) |
| Canopy | CanopyData | animationPath | Canopy animation node path. | string |
| Canopy | CanopyData | animationSpeed | Canopy animation playback speed. | float |
| Canopy | CanopyData | dragWhenOpen | Additional drag when the canopy is open. | float |
| Canopy | CanopyData | insideSubmesh | Submesh index used on the inside of the canopy. | int |
| Canopy | CanopyData | meshPath | Target mesh path. | string |
| Canopy | CanopyData | name | Custom name. | string |
| Canopy | CanopyData | opacity | Transparency. | float |
| Canopy | CanopyData | outsideSubmesh | Submesh index used on the outside of the canopy. | int |
| Canopy | CanopyData | showInside | Whether to display the inner canopy glass. | bool |
| Car Engine | CarEngineData | fuelConsumptionRate | Fuel consumption rate. | float |
| Car Engine | CarEngineData | power | Power/thrust output. | float |
| Car Engine | CarEngineData | throttleResponse | Throttle response speed. | float |
| Catapult Connector | CatapultConnectorData | catapultAcceleration | Catapult acceleration multiplier. | float |
| Catapult Connector | CatapultConnectorData | targetLaunchSpeed | Target launch speed after catapult release. | float |
| Cockpit | CockpitData | hasCamera | Whether this cockpit provides a camera view. | bool |
| Cockpit | CockpitData | lookBackTranslation | Camera translation offset when looking behind the cockpit. | Vector2(x,y) |
| Cockpit | CockpitData | primaryCockpit | Whether this is the primary cockpit. | bool |
| Cockpit Sound | CockpitSoundData | activationGroup | Activation group used for grouped key/control triggering. | string (AlwaysOn, AlwaysOff, 1~8) |
| Cockpit Sound | CockpitSoundData | intensity | Effect strength. | float |
| Control Base | ControlBaseData | attachPointId | Attach-point ID bound to the control base in Joint mode. | int |
| Control Base | ControlBaseData | axis | Control axis direction vector. | Vector3(x,y,z) |
| Control Base | ControlBaseData | haptics | Whether to enable tactile feedback. | bool |
| Control Base | ControlBaseData | ignoreAircraftCollisions | Whether the base ignores collisions with the aircraft. | bool |
| Control Base | ControlBaseData | input | Input axis/button ID. | string |
| Control Base | ControlBaseData | max | Axial input upper limit. | float |
| Control Base | ControlBaseData | min | Axial input lower limit. | float |
| Control Base | ControlBaseData | mode | Control base mode (joint drive or target transformation drive). | Enum(ControlMode: Joint, Transform) |
| Control Base | ControlBaseData | name | Custom name. | string |
| Control Base | ControlBaseData | positionDamper | Translational drive damping. | float |
| Control Base | ControlBaseData | positionMaximumForce | Translation drive maximum force. | float |
| Control Base | ControlBaseData | positionSpring | Translation drive spring stiffness. | float |
| Control Base | ControlBaseData | rotationMaxDistance | Maximum deflection distance of rotation axis. | float |
| Control Base | ControlBaseData | scale | Scale factor. | float |
| Control Base | ControlBaseData | slerpDamper | Angle drive damping. | float |
| Control Base | ControlBaseData | slerpMaximumForce | Angle drive maximum force. | float |
| Control Base | ControlBaseData | slerpSpring | Angle drive spring stiffness. | float |
| Control Base | ControlBaseData | targetTransformPath | Transform mode target node path. | string |
| Control Base | ControlBaseData | v | State version number. | int |
| Control Surface | ControlSurfacePartData | dummyPartFlipped | Whether to flip the control surface when mirroring. | bool |
| Control Surface | ControlSurfacePartData | dummyWingOffset | Control surface wing offset cache. | Vector2(x,y) |
| Control Surface | ControlSurfacePartData | dummyWingScale | Control surface wing-associated scaling cache. | Vector2(x,y) |
| Control Surface | ControlSurfacePartData | style | Style preset. | string |
| Countermeasure Dispenser | CounterMeasureDispenserData | activationGroup | Activation group used for grouped key/control triggering. | int |
| Countermeasure Dispenser | CounterMeasureDispenserData | ammo | Number of countermeasures available. | int |
| Countermeasure Dispenser | CounterMeasureDispenserData | autoDispenseDelay | Interval time between automatic release of countermeasures (seconds). | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | breakLockChance | The probability of the missile breaking lock after interference. | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | evadeLockChance | Probability of evading locking after interference. | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | launchForce | Countermeasure launch force. | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | type | Countermeasure type. | Enum(CounterMeasureType: None, Flares, Chaff) |
| Decal | DecalData | color | Decal color (tint). | Color(HEX RGB) |
| Decal | DecalData | decalRotation | Decal Euler rotation angle. | Vector3(x,y,z) |
| Decal | DecalData | opacity | Transparency. | float |
| Decal | DecalData | partIds | Target part ID list. | int list (comma separated) |
| Decal | DecalData | penetration | Decal throw depth/penetration factor. | float |
| Decal | DecalData | priority | Decal rendering priority. | int |
| Decal | DecalData | size | Decal size scale factor. | Vector3(x,y,z) |
| Decal | DecalData | target | Decal target mode. | string (Single Part/MultipleParts) |
| Decal | TextureDecalData | decalId | Decal Texture ID. | string |
| Decal | TextureDecalData | offset | Position offset vector. | Vector2(x,y) |
| Decal | TextureDecalData | tiling | Decal tiling ratio. | Vector2(x,y) |
| Detacher | DetacherData | attachPointsToDetach | List of connection point IDs to disconnect when triggering detachment. | int list (comma separated) |
| Detacher | DetacherData | delay | Detach trigger delay (seconds). | float |
| Detacher | DetacherData | detacherUiMaxForce | Maximum separation force adjustable by separator UI. | float |
| Detacher | DetacherData | detachForce | Actual applied separation force. | float |
| Detacher | DetacherData | direction | Separate force direction. | Enum(DetacherDirection: Default, Forward) |
| Detacher | DetacherData | enabled | Whether this feature is enabled. | bool |
| Detacher | DetacherData | group | Activation group assigned to the detacher. | string (0/1~8,0=Disabled) |
| Differential | JDifferentialData | coastStiffness | Differential locking response during coast/braking. | float |
| Differential | JDifferentialData | lock | Differential lock ratio. | float |
| Differential | JDifferentialData | powerStiffness | Differential locking response under acceleration. | float |
| Differential | JDifferentialData | size | Size scale factor. | float |
| Drive Shaft | JDriveHubData | reversed | Whether to reverse the direction of rotation. | bool |
| Drive Shaft | JDriveShaftData | bootA | Whether to show the dust boot on drive-shaft end A. | bool |
| Drive Shaft | JDriveShaftData | bootB | Whether to show the dust boot on drive-shaft end B. | bool |
| Drive Shaft | JDriveShaftData | end | Local coordinates of drive shaft end point. | Vector3(x,y,z) |
| Drive Shaft | JDriveShaftData | radius | Radius. | float |
| Drive Shaft | JDriveShaftData | start | Local coordinates of the starting point of the drive shaft. | Vector3(x,y,z) |
| Drive Shaft | JDriveShaftData | visual | Whether to display the visual drive shaft. | bool |
| Engine | EngineData | alphaTiedToThrottle | Whether exhaust flame transparency changes with throttle. | bool |
| Engine | EngineData | ductedThrust | Whether thrust is calculated using ducted-thrust mode. | bool |
| Engine | EngineData | exhaustScale | Exhaust effect scale. | Vector3(x,y,z) |
| Engine | EngineData | fuelConsumptionRate | Fuel consumption rate. | float |
| Engine | EngineData | power | Power/thrust output. | float |
| Engine | EngineData | powerMultiplier | Power multiplier. | float |
| Engine | EngineData | requiredAirIntake | Air intake required to achieve rated output. | float |
| Engine | EngineData | soundOverride | Engine sound effect override ID. | string |
| Engine | EngineData | throttleResponse | Throttle response speed. | float |
| Engine | EngineData | type | Engine implementation type. | Enum(EngineType: Prop, Turbojet, AfterburningTurbojet) |
| Engine | JEngineData | basePower | Engine base power calibration value. | float |
| Engine | JEngineData | baseRpm | Engine base RPM calibration value. | float |
| Engine | JEngineData | baseSize | Engine basic size calibration value. | float |
| Engine | JEngineData | cylinderRows | Number of cylinders per row (or group). | int |
| Engine | JEngineData | engineConfiguration | Engine configuration index (cylinder configuration). | int |
| Engine | JEngineData | engineTuning | Engine tuning tendency (torque ↔ high speed). | float |
| Engine | JEngineData | forcedInduction | Forced-induction ratio. | float |
| Engine | JEngineData | horsePower | Engine horsepower. | float |
| Engine | JEngineData | mass | Engine mass. | float |
| Engine | JEngineData | massToPower | Power to weight ratio coefficient. | float |
| Engine | JEngineData | powerCurve | Engine power curve (serialized string). | string |
| Engine | JEngineData | redLine | Redline RPM ratio. | float |
| Engine | JEngineData | rpm | Maximum engine RPM. | float |
| Engine | JEngineData | rpmScalingExponent | Scaling exponent for the effect of size on rotational speed. | float |
| Engine | JEngineData | size | Engine size scale factor. | float |
| Engine | JEngineData | soundPitchLimit | Upper limit of sound pitch. | float |
| Engine | JEngineData | soundPitchOffset | Sound pitch shift. | float |
| Engine | JEngineData | soundPitchRange | Sound pitch range. | float |
| Engine | JEngineData | soundType | Engine sound type combinations. | Enum(EngineSoundType: None, Prop, Car, Boat, V, Flat, Radial, Inline, Electric, PropV, PropFlat, PropRadial, CarV, CarFlat, CarInline) |
| Engine | JEngineData | startupDuration | Engine startup duration. | float |
| Engine | JEngineData | supercharger | Whether to enable supercharging. | bool |
| Engine | JEngineData | superchargerMultiplier | Supercharger boost multiplier. | float |
| Engine | JEngineData | throttleResponse | Throttle response speed. | float |
| Floating Part | FloatingPartData | enabled | Whether this feature is enabled. | bool |
| Floating Part | FloatingPartData | impactVelocityAdjustment | Water-entry impact velocity adjustment curve (name or constant). | string (curve nameorsingle float value) |
| Floating Part | FloatingPartData | reduceBuoyancyIfBySelf | Whether to reduce buoyancy when surrounding a body of water. | bool |
| Floating Part | FloatingPartData | weightFactor | Buoyancy weight coefficient. | float |
| Fuel Tank | FuelTankData | capacity | Maximum capacity of fuel tank. | float |
| Fuel Tank | FuelTankData | fuel | Current fuel level. | float |
| Fuel Tank | ResizableFuelTankData | capacity | Maximum capacity of fuel tank. | float |
| Fuel Tank | ResizableFuelTankData | size | Fuel tank size scale factor. | float |
| Fuselage | FuselageData | autoSizeOnConnected | Whether to automatically match the cross-section size when connecting to other fuselages. | bool |
| Fuselage | FuselageData | buoyancy | Part buoyancy coefficient. | float |
| Fuselage | FuselageData | collider | Fuselage collision body generation mode. | Enum(FuselageColliderType: Auto, Basic, ConvexMesh, NonConvexMesh) |
| Fuselage | FuselageData | collider | Collider generation mode. | Enum(FuselageData.FuselageColliderType: Auto, Basic, ConvexMesh, NonConvexMesh) |
| Fuselage | FuselageData | cornerTypes | List of fuselage angle types (front and rear sections). | int list (8 items,comma separated) |
| Fuselage | FuselageData | deadWeight | Additional load mass. | float |
| Fuselage | FuselageData | fillBack | Fuselage rear section cutting values (supports single value or four-way value). | float or float4(top,bottom,left,right) |
| Fuselage | FuselageData | fillCutFace | Whether to seal after cutting. | bool |
| Fuselage | FuselageData | fillFront | Fuselage front section cutting values (supports single value or four-way value). | float or float4(top,bottom,left,right) |
| Fuselage | FuselageData | frontScale | Fuselage front section scale. | Vector2(x,y) |
| Fuselage | FuselageData | fuelPercentage | Available fuel ratio of the fuselage. | float |
| Fuselage | FuselageData | inletSlant | Air inlet inclination angle. | float |
| Fuselage | FuselageData | inletThicknessFront | Inlet leading edge thickness. | float |
| Fuselage | FuselageData | inletThicknessRear | Intake trailing edge thickness. | float |
| Fuselage | FuselageData | inletTrimSize | Air intake trim dimensions. | float |
| Fuselage | FuselageData | offset | Position offset. | Vector3(x,y,z) |
| Fuselage | FuselageData | rearScale | Fuselage rear section scale. | Vector2(x,y) |
| Fuselage | FuselageData | smoothBack | Whether back-section normal smoothing is enabled. | bool |
| Fuselage | FuselageData | smoothFront | Whether front-section normal smoothing is enabled. | bool |
| Fuselage | FuselageData | type | Fuselage type identification (fuselage/cone/inlet/hollow/glass, etc.). | string (body, cone, inlet, hollow, glass, hollowglass) |
| Fuselage | FuselageData | version | State version number. | int |
| Fuselage | JFuselageData | autoResize | Whether to automatically adjust the fuselage cross-section size when connecting. | bool |
| Fuselage | JFuselageData | buoyancy | Buoyancy coefficient. | float |
| Fuselage | JFuselageData | colliderCornerSamples | Collider corner point sampling number. | int |
| Fuselage | JFuselageData | cornerRadii | Four corner fillet radius of fuselage section. | Vector4(x,y,z,w) |
| Fuselage | JFuselageData | cornerSamples | Number of samples at four corners of fuselage section. | Int4(x,y,z,w) |
| Fuselage | JFuselageData | cornerStretch | Whether fuselage section corner stretching is enabled. | Bool4(x,y,z,w) |
| Fuselage | JFuselageData | cutting | Fuselage section cutting values. | decimal?list (4 items,comma separated,optional blank) |
| Fuselage | JFuselageData | deadMassKg | Additional dead weight (kg). | float |
| Fuselage | JFuselageData | defaultThicknessFront | Default thickness of front section. | float |
| Fuselage | JFuselageData | defaultThicknessRear | Back section default thickness. | float |
| Fuselage | JFuselageData | edgeCurvature | Fuselage section edge curvature. | Vector4(x,y,z,w) |
| Fuselage | JFuselageData | edgeSamples | Number of fuselage section edge samples. | Int4(x,y,z,w) |
| Fuselage | JFuselageData | fuelProportion | Fuel volume ratio. | float |
| Fuselage | JFuselageData | glass | Whether to enable glass material mode. | bool |
| Fuselage | JFuselageData | legacyThickness | Whether to use legacy thickness logic. | bool |
| Fuselage | JFuselageData | mass | Serialized mass and center-of-gravity packing value (x, y, z, mass). | Vector4(x,y,z,w) |
| Fuselage | JFuselageData | noseconeRoundness | The roundness of the cone nose. | float |
| Fuselage | JFuselageData | numColliders | Number of collision body segments. | int |
| Fuselage | JFuselageData | offset | Position offset. | Vector3(x,y,z) |
| Fuselage | JFuselageData | size | Fuselage cross-section size (SectionA/SectionB). | Vector2(x,y) |
| Fuselage | JFuselageData | smoothing | Whether cross-section smoothing is enabled. | bool |
| Fuselage | JFuselageData | style | Style preset. | Enum(FuselageStyle: Body, Hollow, Inlet, Cone, HollowCone) |
| Fuselage | JFuselageData | syncSlices | Whether front and rear section parameters are synchronized. | bool |
| Fuselage | JFuselageData | thickness | Section thickness. | float |
| Fuselage | JFuselageData | trapezium | Cross-section trapezoidal offset. | float |
| Fuselage | JFuselageData | version | State version number. | int |
| Gauge | GaugeData | altitudeUnit | Altimeter unit settings. | Enum(GaugeData.AltitudeUnit: Feet, Meters, None) |
| Gauge | GaugeData | face | Gauge face style. | Enum(GaugeData.GaugeFaceTypes: AirSpeed200Indicator, AirSpeed400Indicator, AirSpeed600Indicator, AltimeterIndicator, AttitudeIndicator, FuelIndicator, HeadingIndicator, ThrottleIndicator, TrimIndicator, TurnCoordinatorIndicator, VerticalSpeedIndicator, VTOLIndicator, RotorRPM, Basic1) |
| Gauge | GaugeData | faceEmission | Legacy field: unified dial emission intensity. | float |
| Gauge | GaugeData | faceEmissionDay | Dial luminous intensity during daytime. | float |
| Gauge | GaugeData | faceEmissionNight | Luminous intensity of dial at night. | float |
| Gauge | GaugeData | faceInput | Dial face rotation input expression. | string |
| Gauge | GaugeData | faceMultiplier | Dial face input magnification. | float |
| Gauge | GaugeData | faceZero | Dial surface zero angle offset. | float |
| Gauge | GaugeData | hideBase | Whether to hide the instrument base. | bool |
| Gauge | GaugeData | hideFace | Whether to hide the dashboard. | bool |
| Gauge | GaugeData | hideTrim | Whether to hide the instrument bezel. | bool |
| Gauge | GaugeData | indicator | Legacy field: pointer style. | Enum(GaugeData.IndicatorType: Indicator1, Indicator2, Indicator3, Indicator4, Indicator5, Indicator6, Indicator7, None) |
| Gauge | GaugeData | indicatorZero | Legacy field: pointer zero-angle offset. | float |
| Gauge | GaugeData | input | Legacy field: pointer input source. | string |
| Gauge | GaugeData | invert | Whether legacy input is inverted. | bool |
| Gauge | GaugeData | multiplier | Legacy field: input multiplier. | float |
| Gauge | GaugeData | rotationType | Rotation mode. | Enum(GaugeData.GaugeRotationType: Indicator, Face) |
| Gauge | GaugeData | scale | Scale factor. | float |
| Gauge | GaugeData | speedUnit | Speed unit setting. | Enum(GaugeData.SpeedUnit: Knots, MetersPerSecond, MilesPerHour, KilometersPerHour, None) |
| Gauge | GaugeData | trimType | Instrument bezel style. | Enum(GaugeData.GaugeTrimType: Trim1, Trim2) |
| Gauge | GaugeData | type | Gauge type preset. | Enum(GaugeData.GaugeTypePreset: Custom, Heading, Fuel, Throttle, Speed200, Speed400, Speed600, Altitude, Trim, TurnCoordinator, VerticalSpeed, RotorRPM, VTOL, BankAngle) |
| Gauge | GaugeData | zero | Legacy field: input zero offset. | float |
| Gearbox | JGearboxData | gearRatio | Gear ratio. | float |
| Gearbox | JGearboxData | reversed | Whether to reverse the output direction. | bool |
| Gearbox | JGearboxData | size | Gearbox size scale factor. | float |
| Gun | GunData | activationGroup | Activation group used for grouped key/control triggering. | string (All, 1~8) |
| Gun | GunData | ammoCount | Total ammunition count. | int |
| Gun | GunData | bulletScale | Bullet model scaling. | Vector3(x,y,z) |
| Gun | GunData | burstCount | Number of bursts per round. | int |
| Gun | GunData | damage | Single shot damage. | float |
| Gun | GunData | impactForce | Impact force on hit. | float |
| Gun | GunData | lifetime | Projectile lifetime (seconds). | float |
| Gun | GunData | muzzleFlash | Whether to enable muzzle flash. | bool |
| Gun | GunData | muzzleVelocity | Muzzle velocity. | float |
| Gun | GunData | roundsPerSecond | Rate of fire per second. | float |
| Gun | GunData | spread | Dispersion angle. | float |
| Gun | GunData | timeBetweenBursts | Burst interval time. | float |
| Gun | GunData | tracerIntensity | Tracer intensity. | float |
| Gyroscope | GyroscopeData | activationGroup | Activation group used for grouped key/control triggering. | string (None, 1~8) |
| Gyroscope | GyroscopeData | autoOrient | Whether to enable automatic attitude maintenance. | bool |
| Gyroscope | GyroscopeData | pitchRange | Pitch stability range. | float |
| Gyroscope | GyroscopeData | rollRange | Roll stability range. | float |
| Gyroscope | GyroscopeData | speed | Response speed. | float |
| Gyroscope | GyroscopeData | stability | Stability coefficient. | float |
| Gyroscope | GyroscopeData | yawPower | Yaw control strength. | float |
| IK Target | IKTargetData | offset | Position offset. | Vector3(x,y,z) |
| IK Target | IKTargetData | path | Target node path. | string |
| IK Target | IKTargetData | positionWeight | IK position weight. | float |
| IK Target | IKTargetData | priority | Priority. | int |
| IK Target | IKTargetData | rotationWeight | IK rotation weight. | float |
| IK Target | IKTargetData | type | IK target type. | Enum(IKTargetType: Body, LeftShoulder, RightShoulder, LeftThigh, RightThigh, LeftHand, RightHand, LeftFoot, RightFoot, LeftElbow, RightElbow, LeftKnee, RightKnee) |
| Inlet | InletData | airIntakeMultiplier | Intake efficiency ratio. | float |
| Input Controller | InputControllerData | activationGroup | Activation group used for grouped key/control triggering. | string (0~8) |
| Input Controller | InputControllerData | defaultActivationGroup | Default activation group used at part initialization. | string (0~8) |
| Input Controller | InputControllerData | defaultInput | Default input channel (as part initial value). | string |
| Input Controller | InputControllerData | defaultMax | Default output upper limit (as part initial value). | float |
| Input Controller | InputControllerData | defaultMin | Default output lower limit (as part initial value). | float |
| Input Controller | InputControllerData | input | Input axis/button ID. | string |
| Input Controller | InputControllerData | invert | Whether input is inverted. | bool |
| Input Controller | InputControllerData | invertOnMirror | Whether to invert input when mirroring a copy. | bool |
| Input Controller | InputControllerData | invertType | How inversion is applied. | Enum(InvertType: Axis, Output) |
| Input Controller | InputControllerData | max | Maximum output value. | float |
| Input Controller | InputControllerData | min | Minimum output value. | float |
| Input Controller | InputControllerData | name | Controller name. | string |
| Input Controller | InputControllerData | propertyEditorDesc | Properties panel display instructions. | string |
| Input Controller | InputControllerData | zeroOnDeactivate | Whether to zero output when deactivating an activation group. | bool |
| Jet Engine | JetEngineData | afterburner | Whether to enable afterburner. | bool |
| Jet Engine | JetEngineData | afterburnerBaseColor | Afterburner tail flame root color. | Color(HTML Hex RGBA) |
| Jet Engine | JetEngineData | afterburnerThrottleStart | Afterburner intervention throttle threshold. | float |
| Jet Engine | JetEngineData | afterburnerTipColor | Afterburner tail flame tip color. | Color(HTML Hex RGBA) |
| Jet Engine | JetEngineData | baseSize | Basic size scaling benchmark. | float |
| Jet Engine | JetEngineData | burnerTemp | Combustion chamber temperature setting. | float |
| Jet Engine | JetEngineData | burnerTempRange | Combustion chamber temperature adjustable range. | float list (2 items: min,max) |
| Jet Engine | JetEngineData | bypassRange | Bypass ratio adjustable range. | float list (2 items: min,max) |
| Jet Engine | JetEngineData | bypassRatio | Bypass ratio. | float |
| Jet Engine | JetEngineData | compressionRange | Compression ratio adjustable range. | float list (2 items: min,max) |
| Jet Engine | JetEngineData | compressionRatio | Compression ratio. | float |
| Jet Engine | JetEngineData | coreVisualScale | Engine core visual scale. | float |
| Jet Engine | JetEngineData | fanPressureRatio | Fan pressure ratio. | float |
| Jet Engine | JetEngineData | fanStyle | Fan style ID. | string |
| Jet Engine | JetEngineData | gimbalSpeed | Nozzle gimbal slew speed. | float |
| Jet Engine | JetEngineData | inletConeStyle | Intake cone style ID. | string |
| Jet Engine | JetEngineData | jetEngineType | Jet engine type. | Enum(JetEngineType: None, Legacy, Civilian, Military) |
| Jet Engine | JetEngineData | mass | Engine mass parameter. | float |
| Jet Engine | JetEngineData | maxGimbalAngle | Maximum nozzle deflection angle ratio. | float |
| Jet Engine | JetEngineData | nozzleLength | Nozzle length coefficient. | float |
| Jet Engine | JetEngineData | nozzleStyle | Nozzle style ID. | string |
| Jet Engine | JetEngineData | reverseThrust | Whether to enable reverse thrust. | bool |
| Jet Engine | JetEngineData | size | Engine size scale factor. | float |
| Jet Engine | JetEngineData | sizeRange | Size adjustable range. | float list (2 items: min,max) |
| Jet Engine | JetEngineData | turbinePressureRatio | Turbine pressure ratio. | float |
| Jet Engine Shroud | JetEngineShroudData | jetEngineType | Jet engine type. | Enum(JetEngineType: None, Legacy, Civilian, Military) |
| Jet Engine Shroud | JetEngineShroudData | length | Length factor. | float |
| Jet Engine Shroud | JetEngineShroudData | radius | Radius value. | float |
| Jet Engine Shroud | JetEngineShroudData | style | Style preset. | string |
| Joint Motor | JointMotorData | attachPoint | Joint motor binding connection point index. | int |
| Joystick | AdjustableJoystickData | colliderPath | Joystick collider node path. | string |
| Joystick | AdjustableJoystickData | cylinderPath | Joystick shaft node path. | string |
| Joystick | AdjustableJoystickData | headPaths | Joystick head node path list. | string list (comma separated node paths) |
| Joystick | AdjustableJoystickData | height | Height value. | float |
| Label | LabelData | curvature | Text bend angle. | float |
| Label | LabelData | curvatureDirection | Text bending direction. | Enum(LabelCurvatureDirection: Horizontal, Vertical) |
| Label | LabelData | designText | Label display text. | string |
| Label | LabelData | emission | Legacy field: unified self-illumination intensity. | float |
| Label | LabelData | emissionDay | Daytime self-illumination intensity. | float |
| Label | LabelData | emissionNight | Self-illumination intensity at night. | float |
| Label | LabelData | fontName | Font name. | string |
| Label | LabelData | fontSize | Font size factor. | float |
| Label | LabelData | gradient | Text gradient style. | Enum(LabelPartGradientType: None, Vertical, Horizontal, Diagonal, UpperLeft, UpperRight, LowerLeft, LowerRight) |
| Label | LabelData | height | Height value. | float |
| Label | LabelData | horizontalAlignment | Text horizontal alignment. | Enum(Left, Center, Right) |
| Label | LabelData | offset | Position offset. | Vector3(x,y,z) |
| Label | LabelData | outlineWidth | Text stroke width. | float |
| Label | LabelData | paintIndexShift | Paint index offset. | int |
| Label | LabelData | parentPath | Label parent node path. | string |
| Label | LabelData | renderQueueOffset | Render queue offset. | int |
| Label | LabelData | supportsCurvature | Whether to support text bending. | bool |
| Label | LabelData | supportsGradient | Whether to support text gradient. | bool |
| Label | LabelData | verticalAlignment | Text vertical alignment. | Enum(Top, Middle, Bottom) |
| Label | LabelData | width | Width value. | float |
| Landing Gear | RetractableLandingGearData | (none) | This part reads no unique attribute in its own state; behavior mainly comes from base/shared logic. | None |
| Landing Gear | WheelData | (none) | This part reads no unique attribute in its own state; behavior mainly comes from base/shared logic. | None |
| Landing Gear | WingLandingGearData | (none) | This part reads no unique attribute in its own state; behavior mainly comes from base/shared logic. | None |
| Magnet | MagnetData | activationGroup | Activation group used for grouped key/control triggering. | string (None, 1~8) |
| Magnet | MagnetData | power | Magnetic strength/power. | float |
| Main Rotor | HeliMainRotorData | centerOfMassOffset | Main rotor system center of mass offset. | Vector3(x,y,z) |
| Main Rotor | HeliMainRotorData | cyclicPitchMaxDeflection | Main rotor periodic pitch maximum deflection angle. | float |
| Main Rotor | HeliMainRotorData | cyclicRollMaxDeflection | Main rotor periodic roll maximum deflection angle. | float |
| Main Rotor | HeliMainRotorData | rotorDamping | Rotor vibration damping coefficient. | float |
| MFD | MfdData | targetingPod | Part ID of the associated targeting pod. | int (target part ID) |
| Missile | MissileData | function | Weapon usage mode. | Enum(WeaponFunction: None, AirToAir, AirToSurface, MultiRole) |
| Missile | MissileData | guidanceActivationDelay | Guidance activation delay. | float |
| Missile | MissileData | ignitionDelay | Ignition delay. | float |
| Missile | MissileData | killCam | Whether to enable the kill camera after a hit. | bool |
| Missile | MissileData | loft | Missile parabolic climb ratio (Loft). | float |
| Missile | MissileData | maxForwardThrustForce | Maximum forward thrust. | float |
| Missile | MissileData | maxFuelTime | Maximum burning time. | float |
| Missile | MissileData | maxHeadingAngleAdjustmentRate | Maximum course correction rate. | float |
| Missile | MissileData | maxRange | Maximum effective range. | float |
| Missile | MissileData | maxSpeed | Maximum speed. | float |
| Missile | MissileData | maxTargetingAngle | Maximum locking angle. | float |
| Missile | MissileData | maxThrustVectoringRate | Maximum thrust vector correction rate. | float |
| Missile | MissileData | maxTorque | Maximum torque. | float |
| Missile | MissileData | maxVelocityAngleAdjustmentRate | Maximum velocity vector correction rate. | float |
| Missile | MissileData | minRange | Minimum effective range. | float |
| Missile | MissileData | proximityDetonationRangeMax | Maximum triggering distance of proximity fuze. | float |
| Missile | MissileData | proximityDetonationRangeMin | Minimum triggering distance of proximity fuze. | float |
| Missile | MissileData | seeker | Seeker type. | Enum(SeekerType: Unguided, Infrared, SemiActiveRadar, ActiveRadar, Laser, AntiRadiation) |
| Missile | MissileData | smokeOpacity | Tail smoke opacity. | float |
| Missile | MissileData | smokeScale | Tail smoke scale. | float |
| Missile | MissileData | waterproof | Whether the missile is waterproof. | bool |
| Missile Configuration | ProceduralMissileData | attachPosition | The front and rear installation positions of the missile on the hardpoint. | float (-1~1) |
| Missile Configuration | ProceduralMissileData | body | Procedural missile body-segment style ID. | string |
| Missile Configuration | ProceduralMissileData | burnTime | Engine combustion time ratio. | float (0~1) |
| Missile Configuration | ProceduralMissileData | engine | Missile engine type. | Enum(MissileEngineType: Solid, ThrustVector, Jet) |
| Missile Configuration | ProceduralMissileData | nose | Procedural missile nose-cone style ID (optional override). | string |
| Missile Configuration | ProceduralMissileData | noseLength | Missile nose length. | float |
| Missile Configuration | ProceduralMissileData | radius | Radius / effective radius. | float |
| Missile Configuration | ProceduralMissileData | seeker | Seeker type configuration. | Enum(SeekerType: Unguided, Infrared, SemiActiveRadar, ActiveRadar, Laser, AntiRadiation) |
| Missile Configuration | ProceduralMissileData | seekerFOV | Seeker field-of-view angle. | float |
| Missile Configuration | ProceduralMissileData | size | Missile size. | float |
| Missile Configuration | ProceduralMissileData | updateMissileModifier | Whether missile modifiers are refreshed after parameter changes. | bool |
| Missile Configuration | ProceduralMissileData | warheadBias | Warhead bias/placement parameter. | float |
| Nosecone | AdaptiveNoseConeData | scale | Scaling ratio/factor. | Vector3(x,y,z) |
| Parachute | ParachuteData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Parachute | ParachuteData | size | Parachute size. | float |
| Parachute | ParachuteData | style | Style preset. | string |
| Part Targeting | PartTargetingData | customPartIds | Custom target part ID list. | int list (comma separated) |
| Part Targeting | PartTargetingData | partIds | Referenced part ID list. | int list (comma separated) |
| Part Targeting | PartTargetingData | targetMode | Part targeting mode. | Enum(PartTargetingMode: SinglePart, MultipleParts, Custom) |
| Pedal | PedalData | fullAngle | Full travel angle. | float |
| Pedal | PedalData | input | Input source/controller binding name. | string |
| Pedal | PedalData | zeroAngle | Zero position angle. | float |
| Piston | PistonData | attachPoint | Attach point index for the piston moving end. | int |
| Piston | PistonData | cycle | Whether the piston cycles repeatedly. | bool |
| Piston | PistonData | extend | Whether the piston uses extend (push) mode. | bool |
| Piston | PistonData | maxRange | Maximum range value. | float |
| Piston | PistonData | maxSpeed | Maximum speed limit. | float |
| Piston | PistonData | preventBreaking | Whether to prevent joint breakage under load. | bool |
| Piston | PistonData | range | Operating range. | float |
| Piston | PistonData | speed | Speed setting. | float |
| Posed Grip | PosedGripData | asButton | Whether input is treated as button mode. | bool |
| Posed Grip | PosedGripData | colliders | Collider path list (comma separated). | string |
| Posed Grip | PosedGripData | control | Control binding name. | string |
| Posed Grip | PosedGripData | controlPath | XR control path. | string |
| Posed Grip | PosedGripData | disableTooltip | Whether tooltip display is disabled. | bool |
| Posed Grip | PosedGripData | gripTarget | Grip target transform path. | string |
| Posed Grip | PosedGripData | gripType | XR grip control scheme (ungripped / primary / secondary). | Enum(XRControlGripType: Default/FlightStick/Throttle) |
| Posed Grip | PosedGripData | outlineScale | Scale factor. | Vector3(x,y,z) |
| Posed Grip | PosedGripData | pose | Grip pose name. | string |
| Posed Grip | PosedGripData | previewPose | Preview pose in editor. | string |
| Posed Grip | PosedGripData | processor | Input processor expression. | string |
| Posed Grip | PosedGripData | tooltip | Tooltip text. | string |
| Posed Grip | PosedGripData | tooltipOffset | Tooltip offset value. | float |
| Posed Grip | PosedGripData | tooltipTransformPath | Tooltip anchor transform path. | string |
| Procedural Bay | ProceduralBayData | doorStyle | Door opening style. | Enum(DoorStyle: None, SingleLeft, SingleRight, Double) |
| Procedural Bay | ProceduralBayData | startOpen | Whether the part starts open. | bool |
| Procedural Window | ProceduralWindowData | hideGlass | Whether to hide the glass layer. | bool |
| Propeller Engine | PropEngineAdvancedData | legacyCotPos | Whether to use legacy center-of-thrust position logic. | bool |
| Propellers | PropellerAssemblyData | bladeBlurCount | Number of blade blur segments. | int |
| Propellers | PropellerAssemblyData | bladeBlurSpread | Blade blur spread range. | float |
| Propellers | PropellerAssemblyData | bladeCount | Blade count. | int |
| Propellers | PropellerAssemblyData | chordRadiusRatio | Chord-to-radius ratio. | float |
| Propellers | PropellerAssemblyData | chordScale | Blade chord scale. | float |
| Propellers | PropellerAssemblyData | defaultDiameter | Default propeller diameter. | float |
| Propellers | PropellerAssemblyData | density | Density parameter. | float |
| Propellers | PropellerAssemblyData | dragScalar | Drag scale factor. | float |
| Propellers | PropellerAssemblyData | hub | Hub style or resource id. | string |
| Propellers | PropellerAssemblyData | hubScale | Hub scale factor. | float |
| Propellers | PropellerAssemblyData | isWaterProp | Whether this is a water prop. | bool |
| Propellers | PropellerAssemblyData | magicEngineId | Linked engine identifier. | int |
| Propellers | PropellerAssemblyData | maxPitch | Maximum pitch angle. | float |
| Propellers | PropellerAssemblyData | pitchControlType | Propeller pitch control mode. | Enum(PropellerAssemblyData.PitchControl: Auto, Fixed, Manual) |
| Propellers | PropellerAssemblyData | propeller | Propeller style/resource id. | string |
| Propellers | PropellerAssemblyData | pushProp | Whether to use a pusher configuration. | bool |
| Propellers | PropellerAssemblyData | reverseBladeDirection | Whether blade rotation direction is reversed. | bool |
| Propellers | PropellerAssemblyData | size | Propeller size. | float |
| Propellers | PropellerAssemblyData | thrustScalar | Thrust scale factor. | float |
| Propellers | PropellerAssemblyData | twistAngleRoot | Root blade twist angle. | float |
| Reaction Control Nozzle | ReactionControlNozzleData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Reaction Control Nozzle | ReactionControlNozzleData | autoAssignType | Whether nozzle control axis type is auto-detected. | bool |
| Reaction Control Nozzle | ReactionControlNozzleData | fuelConsumptionRate | Fuel consumption rate. | float |
| Reaction Control Nozzle | ReactionControlNozzleData | power | Power/strength output parameter. | float |
| Reaction Control Nozzle | ReactionControlNozzleData | reverse | Whether output direction is reversed. | bool |
| Reaction Control Nozzle | ReactionControlNozzleData | type | RCS nozzle axis type (pitch / roll / yaw). | Enum(ReactionControlNozzleType: Pitch/Roll/Yaw) |
| Refuel Drouge | RefuelDrogueData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Refuel Drouge | RefuelDrogueData | angularDragPower | Angular drag strength. | float |
| Refuel Drouge | RefuelDrogueData | angularStabPower | Angular stabilization strength. | float |
| Refuel Drouge | RefuelDrogueData | transferRate | Transfer rate. | float |
| Refuel Drouge | RefuelDrogueData | triggerColliderPath | Trigger collider path. | string |
| Refuel Probe | RefuelProbeData | offset | Position offset. | Vector2(x,y) |
| Resizable Shape | ResizableShapeData | attachPointPosition | Attach point position. | Vector3(x,y,z) |
| Resizable Shape | ResizableShapeData | bounciness | Bounciness coefficient. | float |
| Resizable Shape | ResizableShapeData | friction | Friction coefficient. | float |
| Resizable Shape | ResizableShapeData | size | Raw size value of resizable sphere; runtime visual radius equals value/4. | float (runtime radius = value/4) |
| Rocket | RocketWeaponData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Rocket | RocketWeaponData | burnTimer | Burn timer setting. | float |
| Rocket | RocketWeaponData | explosionScale | Explosion scale factor. | float |
| Rocket | RocketWeaponData | finMode | Fin mode/config marker. | string |
| Rocket | RocketWeaponData | firingDelay | Firing delay. | float |
| Rocket | RocketWeaponData | laserGuided | Whether laser guidance is enabled. | bool |
| Rocket | RocketWeaponData | name | Custom rocket weapon name. | string |
| Rocket | RocketWeaponData | selfDestructTimer | Self-destruct timer. | float |
| Rocket Pod | RocketPodData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Rocket Pod | RocketPodData | explosionScale | Explosion scale factor. | float |
| Rocket Pod | RocketPodData | firingDelay | Firing delay. | float |
| Rocket Pod | RocketPodData | laserGuided | Whether laser guidance is enabled. | bool |
| Rocket Pod | RocketPodData | name | Custom rocket pod name. | string |
| Rotator | JointRotatorData | allowFreeSpin | Whether free spinning is allowed. | bool |
| Rotator | JointRotatorData | attachPoint | Attach point index used by the rotator joint. | int |
| Rotator | JointRotatorData | audio | Whether rotation audio is enabled. | bool |
| Rotator | JointRotatorData | damperMultiplier | Damper multiplier. | float |
| Rotator | JointRotatorData | disableBaseMesh | Whether the base mesh is hidden. | bool |
| Rotator | JointRotatorData | hingeOffset | Hinge offset. | Vector3(x,y,z) |
| Rotator | JointRotatorData | maxRange | Maximum range value. | int |
| Rotator | JointRotatorData | maxSpeed | Maximum speed limit. | float |
| Rotator | JointRotatorData | minRange | Minimum range value. | int |
| Rotator | JointRotatorData | range | Operating range. | float |
| Rotator | JointRotatorData | shortestAngle | Whether rotation uses the shortest angle path. | bool |
| Rotator | JointRotatorData | speed | Speed setting. | float |
| Rotator | JointRotatorData | supportsDisableBaseMesh | Whether base mesh hiding is supported. | bool |
| Seat | SeatData | animation | Animation state/resource name. | string |
| Seat | SeatData | exitPosition | Exit position. | Vector3(x,y,z) |
| Seat | SeatData | exitRotation | Exit rotation. | Vector3(x,y,z) |
| Seat | SeatData | primarySeat | Whether this is the primary seat. | bool |
| Seat | SeatData | reclination | Seat recline amount. | float |
| Seat | SeatData | seatedPosition | Seated position. | Vector3(x,y,z) |
| Seat | SeatData | seatedRotation | Seated rotation. | Vector3(x,y,z) |
| Seat IK | IKSeatData | bodyTarget | Body IK target. | int |
| Seat IK | IKSeatData | designerCharacter | Designer character id. | string |
| Seat IK | IKSeatData | fpvTracking | Whether first-person tracking is enabled. | bool |
| Seat IK | IKSeatData | leftElbowTarget | Left elbow IK target. | int |
| Seat IK | IKSeatData | leftFootTarget | Left foot IK target. | int |
| Seat IK | IKSeatData | leftHandTarget | Left hand IK target. | int |
| Seat IK | IKSeatData | leftKneeTarget | Left knee IK target. | int |
| Seat IK | IKSeatData | leftShoulderTarget | Left shoulder IK target. | int |
| Seat IK | IKSeatData | maintainHeadRotation | Head rotation retention weight. | float |
| Seat IK | IKSeatData | rightElbowTarget | Right elbow IK target. | int |
| Seat IK | IKSeatData | rightFootTarget | Right foot IK target. | int |
| Seat IK | IKSeatData | rightHandTarget | Right hand IK target. | int |
| Seat IK | IKSeatData | rightKneeTarget | Right knee IK target. | int |
| Seat IK | IKSeatData | rightShoulderTarget | Right shoulder IK target. | int |
| Seat IK | IKSeatData | selfAssignTargets | Whether IK targets are assigned automatically. | bool |
| Seat IK | IKSeatData | snapRange | IK snap range. | float |
| Suspension | SuspensionData | attachPoint | Attach point index used by the suspension. | int |
| Suspension | SuspensionData | damper | Damping factor. | float |
| Suspension | SuspensionData | spring | Spring stiffness. | float |
| Switch | CockpitSwitchData | angleOff | Off-state angle. | float |
| Switch | CockpitSwitchData | angleOn | On-state angle. | float |
| Switch | CockpitSwitchData | axis | Axis mapping. | Vector3(x,y,z) |
| Switch | CockpitSwitchData | disableTooltip | Whether tooltip display is disabled. | bool |
| Switch | CockpitSwitchData | inputId | Input identifier. | string |
| Switch | CockpitSwitchData | outputValue | Output value. | float |
| Switch | CockpitSwitchData | positionTransitionDelay | Position transition delay. | float |
| Switch | CockpitSwitchData | positionTransitionTime | Position transition duration. | float |
| Switch | CockpitSwitchData | scale | Scale factor. | float |
| Switch | CockpitSwitchData | style | Style preset. | Enum(CockpitSwitchData.CockpitSwitchStyle: Default, Flip, Rocker, Pivot) |
| Switch | CockpitSwitchData | tooltip | Tooltip text. | string |
| Tail Rotor | HeliTailRotorData | linkageSpeed | Linkage response speed. | float |
| Tail Rotor | HeliTailRotorData | pidGainsHeadingHold | PID gains for heading hold. | Vector3(x,y,z) |
| Tail Rotor | HeliTailRotorData | pidGainsRate | PID gains for rate control. | Vector3(x,y,z) |
| Tail Rotor | HeliTailRotorData | tailMode | Tail rotor mode. | Enum(HeliTailRotorData.TailModeType: HeadingHold, Rate, Manual) |
| Tail Rotor | HeliTailRotorData | tailSpeed | Tail response speed. | float |
| Tail Rotor | HeliTailRotorData | trimScale | Trim scale factor. | float |
| Targeting Pod | TargetingPodData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Targeting Pod | TargetingPodData | defaultActivationGroup | Default activation group on initialization. | string |
| Targeting Pod | TargetingPodData | maxDistance | Maximum effective distance. | float |
| Targeting Pod | TargetingPodData | offset | Position offset. | Vector3(x,y,z) |
| Text Decal | TextDecalData | alignH | Horizontal text alignment. | Enum(TextDecalData.HorizontalTextAlignment: Center, Left, Right, Stretch) |
| Text Decal | TextDecalData | alignV | Vertical text alignment. | Enum(TextDecalData.VerticalTextAlignment: Center, Top, Bottom) |
| Text Decal | TextDecalData | font | Font style. | Enum(TextDecalData.FontStyle: Default, Roboto, Military, FourteenSegment, Stencil) |
| Text Decal | TextDecalData | fontSize | Font size. | float |
| Text Decal | TextDecalData | text | Displayed text. | string |
| Thrust Port | EngineThrustPortData | exhaustScale | Exhaust effect scale. | Vector3(x,y,z) |
| Torpedo | TorpedoData | (none) | No unique attribute is read by this part in its own state; behavior comes from base/shared logic. | None |
| Transmission | JTransmissionData | customGearRatios | Custom gear ratio list. | float list (comma separated) |
| Transmission | JTransmissionData | finalGearRatio | Final drive ratio. | float |
| Transmission | JTransmissionData | gearProfile | Gear profile preset. | Enum(JTransmissionData.JGearProfileType: Street, Racing, Offroad, Custom) |
| Transmission | JTransmissionData | gearTuning | Gear tuning factor. | float |
| Transmission | JTransmissionData | numGears | Number of gears. | int |
| Transmission | JTransmissionData | postShiftBan | Post-shift lockout duration. | float |
| Transmission | JTransmissionData | reverseGearRatio | Reverse gear ratio. | float |
| Transmission | JTransmissionData | shiftDownRpm | Downshift RPM threshold. | float |
| Transmission | JTransmissionData | shiftDuration | Shift duration. | float |
| Transmission | JTransmissionData | shiftGuardSpeedThreshold | Shift guard speed threshold. | float |
| Transmission | JTransmissionData | shiftUpRpm | Upshift RPM threshold. | float |
| Transmission | JTransmissionData | size | Transmission size. | float |
| Transmission | JTransmissionData | transmissionType | Transmission type. | Enum(JTransmissionData.JTransmissionType: Automatic, Manual) |
| Transmission | JTransmissionData | variableShift | Variable shift strategy parameter. | float |
| Transparency | TransparencyData | alwaysFindConnected | Whether connected parts are always included when evaluating transparency. | bool |
| Transparency | TransparencyData | hideBack | Whether back faces are hidden. | bool |
| Transparency | TransparencyData | hideFront | Whether front faces are hidden. | bool |
| Transparency | TransparencyData | hideInside | Whether inside faces are hidden. | bool |
| Transparency | TransparencyData | opacity | Opacity value. | float |
| Transparency | TransparencyData | overrideHide | Whether default hide behavior is overridden. | bool |
| Wheel | JWheelData | brake | Brake strength. | float |
| Wheel | JWheelData | duals | Whether a dual wheel/tire setup is used. | bool |
| Wheel | JWheelData | forcePoint | Force application point parameter. | float |
| Wheel | JWheelData | frictionCirclePower | Friction circle power. | float |
| Wheel | JWheelData | frictionCircleStrength | Friction circle strength. | float |
| Wheel | JWheelData | frictionPreset | Friction preset id/name. | string |
| Wheel | JWheelData | hideRims | Whether rims are hidden. | bool |
| Wheel | JWheelData | magicEngineId | Linked engine identifier. | int |
| Wheel | JWheelData | reversed | Whether wheel direction is reversed. | bool |
| Wheel | JWheelData | rim | Rim style. | string |
| Wheel | JWheelData | rimOffset | Rim offset. | float |
| Wheel | JWheelData | size | Wheel size. | float |
| Wheel | JWheelData | tire | Tire style. | string |
| Wheel | JWheelData | tractionForward | Forward traction coefficient. | float |
| Wheel | JWheelData | tractionSideways | Sideways traction coefficient. | float |
| Wheel | JWheelData | turningAngle | Maximum steering angle. | float |
| Wheel | JWheelData | turningAngleDampening | Steering angle dampening. | float |
| Wheel | JWheelData | turningRate | Steering rate. | float |
| Wheel | JWheelData | width | Wheel width scale. | float |
| Wheel | ResizableWheelData | brakeTorque | Brake torque. | float |
| Wheel | ResizableWheelData | damper | Damping factor. | float |
| Wheel | ResizableWheelData | direction | Drive/rotation direction. | string |
| Wheel | ResizableWheelData | enableAutoTraction | Whether automatic traction control is enabled. | bool |
| Wheel | ResizableWheelData | enableSuspension | Whether the suspension system is enabled. | bool |
| Wheel | ResizableWheelData | engineId | Engine identifier. | int |
| Wheel | ResizableWheelData | hideRims | Whether rims are hidden. | bool |
| Wheel | ResizableWheelData | maxAngularVelocity | Maximum angular velocity. | float |
| Wheel | ResizableWheelData | size | Wheel size. | float |
| Wheel | ResizableWheelData | slipForwardAsymptote | Forward slip asymptote. | float |
| Wheel | ResizableWheelData | slipForwardExtremum | Forward slip extremum. | float |
| Wheel | ResizableWheelData | slipSidewaysAsymptote | Side slip asymptote. | float |
| Wheel | ResizableWheelData | slipSidewaysExtremum | Side slip extremum. | float |
| Wheel | ResizableWheelData | spring | Spring stiffness. | float |
| Wheel | ResizableWheelData | tire | Tire style. | string |
| Wheel | ResizableWheelData | tractionForward | Forward traction coefficient. | float |
| Wheel | ResizableWheelData | tractionSideways | Sideways traction coefficient. | float |
| Wheel | ResizableWheelData | turningAngle | Maximum steering angle. | float |
| Wheel | ResizableWheelData | turningRate | Steering rate. | float |
| Wheel | ResizableWheelData | width | Wheel width scale. | float |
| Wheel Suspension | JWheelSuspensionData | damper | Damping factor. | float |
| Wheel Suspension | JWheelSuspensionData | extension | Suspension extension. | float |
| Wheel Suspension | JWheelSuspensionData | rideHeight | Ride height. | float |
| Wheel Suspension | JWheelSuspensionData | shockPosition | Shock position. | float |
| Wheel Suspension | JWheelSuspensionData | size | Suspension size. | float |
| Wheel Suspension | JWheelSuspensionData | stiffness | Stiffness coefficient. | float |
| Wheel Suspension | JWheelSuspensionData | suspensionLength | Suspension travel length. | float |
| Winch | WinchData | attachPoint | Attach point index used by the winch cable end. | int |
| Winch | WinchData | breakScale | Break threshold scale. | float |
| Winch | WinchData | range | Operating range. | float |
| Winch | WinchData | speed | Speed setting. | float |
| Winch | WinchData | startRange | Initial cable/range value. | float |
| Winch | WinchData | volume | Volume parameter. | float |
| Wing | JWingData | axis | Axis mapping. | string |
| Wing | JWingData | chordSamples | Chord sampling count. | int |
| Wing | JWingData | colliderSamples | Collider sampling count. | int |
| Wing | JWingData | disableWingtipVortices | Whether wingtip vortices are disabled. | bool |
| Wing | JWingData | flipped | Whether airfoil orientation is flipped. | bool |
| Wing | JWingData | fuelFraction | Fuel fraction. | float |
| Wing | JWingData | invert | Whether output is inverted. | bool |
| Wing | JWingData | invertOnMirror | Whether output is inverted on mirrored parts. | bool |
| Wing | JWingData | liftScale | Lift scale factor. | float |
| Wing | JWingData | partIds | Referenced part ID list. | string |
| Wing | JWingData | style | Wing style compatibility field used mainly for migration/legacy data. | string (legacy compatible style marker) |
| Wing | JWingData | version | Serialized data version. | int |
| Wing | JWingData | viscousDragScale | Viscous drag scale factor. | float |
| Wing | JWingData | zeroLiftDragScale | Zero-lift drag scale. | float |
| Wing | WingData | airfoil | Airfoil type. | string |
| Wing | WingData | allowControlSurfaces | Whether control surface usage is allowed. | bool |
| Wing | WingData | angleOfAttack | Angle of attack parameter. | float |
| Wing | WingData | baseThickness | Base/root thickness. | float |
| Wing | WingData | density | Density parameter. | float |
| Wing | WingData | fuelPercentage | Fuel percentage. | float |
| Wing | WingData | hingeDistance | Hinge distance. | float |
| Wing | WingData | inverted | Whether the wing is inverted. | bool |
| Wing | WingData | liftScale | Lift scale factor. | float |
| Wing | WingData | minSectionLength | Minimum section length. | float |
| Wing | WingData | rootLeadingOffset | Root leading-edge offset. | float |
| Wing | WingData | rootTrailingOffset | Root trailing-edge offset. | float |
| Wing | WingData | tipLeadingOffset | Tip leading-edge offset. | float |
| Wing | WingData | tipPosition | Tip position. | Vector3(x,y,z) |
| Wing | WingData | tipThickness | Tip thickness. | float |
| Wing | WingData | tipTrailingOffset | Tip trailing-edge offset. | float |
