## Part XML Attribute Documentation
- Total part types: 83
- Total attribute rows: 654
- Parts without unique attributes: 5

| Part Category | Part Class | Attribute | Description | Input Type |
| --- | --- | --- | --- | --- |
| Advanced Performance Scalars | RotorPerfScalarsData | collectiveDrag | Power/aerodynamics/physics parameter. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | collectiveLift | Power/aerodynamics/physics parameter. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | collectiveTorque | Power/aerodynamics/physics parameter. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicMotorDragTorque | Power/aerodynamics/physics parameter. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicPitchInputExpo | Configures cyclicPitchInputExpo for RotorPerfScalarsData. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicRollInputExpo | Configures cyclicRollInputExpo for RotorPerfScalarsData. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicRpmFalloffExpo | Speed or timing related setting. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | cyclicStrength | Configures cyclicStrength for RotorPerfScalarsData. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | groundEffect | Configures groundEffect for RotorPerfScalarsData. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | gyroscopicLag | Configures gyroscopicLag for RotorPerfScalarsData. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | gyroscopicStabilization | Configures gyroscopicStabilization for RotorPerfScalarsData. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | relativeWindPassiveLift | Power/aerodynamics/physics parameter. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | relativeWindPassiveTorque | Power/aerodynamics/physics parameter. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | relativeWindPeakSpeed | Speed or timing related setting. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | rotorTensor | Configures rotorTensor for RotorPerfScalarsData. | float |
| Advanced Performance Scalars | RotorPerfScalarsData | translationalLift | Power/aerodynamics/physics parameter. | float |
| Airbrake | AirBrakeData | drag | Power/aerodynamics/physics parameter. | float |
| Arresting Hook | ArrestingHookData | activationGroup | Activation group setting for grouped key/control triggering. | string (1~8) |
| Arresting Hook | ArrestingHookData | cableDeceleration | Configures cableDeceleration for ArrestingHookData. | float |
| Arresting Hook | ArrestingHookData | deployedAngle | Rotation/angle related setting. | float |
| Attitude Ball | AttitudeBallData | meshPath | Position/path/target related setting. | string |
| Attitude Ball | AttitudeBallData | rotationType | Rotation/angle related setting. | Enum(AttitudeBallData.BallType: None, Roll, Pitch, Heading, Attitude, LevelCompass, AllAxis) |
| Attitude Ball | AttitudeBallData | scale | Size/scale related setting. | float |
| Beacon Light | BeaconLightData | activationGroup | Activation group setting for grouped key/control triggering. | int (0~8,0=All) |
| Beacon Light | BeaconLightData | blinkProgram | Configures blinkProgram for BeaconLightData. | float list (comma separated seconds) |
| Beacon Light | BeaconLightData | designerBlinkProgram | Configures designerBlinkProgram for BeaconLightData. | Enum(Preset: Steady, Slow Blink, Quick Blink) |
| Beacon Light | BeaconLightData | input | Configures input for BeaconLightData. | string |
| Beacon Light | BeaconLightData | intensity | Configures intensity for BeaconLightData. | float |
| Beacon Light | BeaconLightData | showHalo | Configures showHalo for BeaconLightData. | bool |
| Bomb | BombData | (none) | This part reads no unique attribute in its own state; behavior mainly comes from base/shared logic. | None |
| Button | CockpitButtonData | depthBase | Configures depthBase for CockpitButtonData. | float |
| Button | CockpitButtonData | depthOff | Configures depthOff for CockpitButtonData. | float |
| Button | CockpitButtonData | depthOn | Configures depthOn for CockpitButtonData. | float |
| Button | CockpitButtonData | disableTooltip | Naming/text/interaction display setting. | bool |
| Button | CockpitButtonData | height | Configures height for CockpitButtonData. | float |
| Button | CockpitButtonData | inputId | Identifier/count related setting. | string |
| Button | CockpitButtonData | lightStrength | Configures lightStrength for CockpitButtonData. | float |
| Button | CockpitButtonData | lightTransitionDelay | Speed or timing related setting. | float |
| Button | CockpitButtonData | lightTransitionTime | Configures lightTransitionTime for CockpitButtonData. | float |
| Button | CockpitButtonData | outputValue | Configures outputValue for CockpitButtonData. | float |
| Button | CockpitButtonData | padding | Configures padding for CockpitButtonData. | float |
| Button | CockpitButtonData | positionTransitionDelay | Position/path/target related setting. | float |
| Button | CockpitButtonData | positionTransitionTime | Position/path/target related setting. | float |
| Button | CockpitButtonData | style | Mode/style selection setting. | Enum(CockpitButtonStyle: Rectangular, Circular) |
| Button | CockpitButtonData | tooltip | Naming/text/interaction display setting. | string |
| Button | CockpitButtonData | width | Size/scale related setting. | float |
| Cannon | CannonData | activationGroup | Activation group setting for grouped key/control triggering. | string (0/1~8,0=All) |
| Cannon | CannonData | ammoCount | Identifier/count related setting. | int |
| Cannon | CannonData | barrelLength | Size/scale related setting. | float |
| Cannon | CannonData | barrelRecoil | Configures barrelRecoil for CannonData. | float |
| Cannon | CannonData | baseLength | Size/scale related setting. | float |
| Cannon | CannonData | diameter | Size/scale related setting. | float |
| Cannon | CannonData | explosionScalar | Configures explosionScalar for CannonData. | float |
| Cannon | CannonData | firingDelay | Speed or timing related setting. | float |
| Cannon | CannonData | flashScale | Size/scale related setting. | float |
| Cannon | CannonData | flashSpace | Configures flashSpace for CannonData. | Enum(ParticleSystemSimulationSpace: Local, World, Custom；Customfalls back to Local) |
| Cannon | CannonData | function | Configures function for CannonData. | Enum(WeaponFunction: None, AirToAir, AirToSurface, MultiRole) |
| Cannon | CannonData | fuseInput | Configures fuseInput for CannonData. | string |
| Cannon | CannonData | impactDamageScalar | Configures impactDamageScalar for CannonData. | float |
| Cannon | CannonData | launchVolume | Configures launchVolume for CannonData. | float |
| Cannon | CannonData | muzzleBrake | Configures muzzleBrake for CannonData. | bool |
| Cannon | CannonData | name | Naming/text/interaction display setting. | string |
| Cannon | CannonData | projectileLifetime | Configures projectileLifetime for CannonData. | float |
| Cannon | CannonData | projectileStyle | Mode/style selection setting. | Enum(CannonData.ProjectileStyle: Sphere, Slug) |
| Cannon | CannonData | projectileType | Mode/style selection setting. | Enum(CannonData.ProjectileType: Basic, Explosive) |
| Cannon | CannonData | projectileVelocity | Configures projectileVelocity for CannonData. | float |
| Cannon | CannonData | recoilForce | Configures recoilForce for CannonData. | float |
| Cannon | CannonData | tracerColor | Configures tracerColor for CannonData. | Color(HTML Hex #RRGGBB/#RRGGBBAA) |
| Cannon | CannonData | tracerLength | Size/scale related setting. | float |
| Cannon | CannonData | tracerSpacing | Configures tracerSpacing for CannonData. | int |
| Canopy | CanopyData | activationGroup | Activation group setting for grouped key/control triggering. | int (0~8) |
| Canopy | CanopyData | animationPath | Position/path/target related setting. | string |
| Canopy | CanopyData | animationSpeed | Speed or timing related setting. | float |
| Canopy | CanopyData | dragWhenOpen | Power/aerodynamics/physics parameter. | float |
| Canopy | CanopyData | insideSubmesh | Identifier/count related setting. | int |
| Canopy | CanopyData | meshPath | Position/path/target related setting. | string |
| Canopy | CanopyData | name | Naming/text/interaction display setting. | string |
| Canopy | CanopyData | opacity | Configures opacity for CanopyData. | float |
| Canopy | CanopyData | outsideSubmesh | Identifier/count related setting. | int |
| Canopy | CanopyData | showInside | Identifier/count related setting. | bool |
| Car Engine | CarEngineData | fuelConsumptionRate | Speed or timing related setting. | float |
| Car Engine | CarEngineData | power | Power/aerodynamics/physics parameter. | float |
| Car Engine | CarEngineData | throttleResponse | Configures throttleResponse for CarEngineData. | float |
| Catapult Connector | CatapultConnectorData | catapultAcceleration | Configures catapultAcceleration for CatapultConnectorData. | float |
| Catapult Connector | CatapultConnectorData | targetLaunchSpeed | Position/path/target related setting. | float |
| Cockpit | CockpitData | hasCamera | Configures hasCamera for CockpitData. | bool |
| Cockpit | CockpitData | lookBackTranslation | Configures lookBackTranslation for CockpitData. | Vector2(x,y) |
| Cockpit | CockpitData | primaryCockpit | Configures primaryCockpit for CockpitData. | bool |
| Cockpit Sound | CockpitSoundData | activationGroup | Activation group setting for grouped key/control triggering. | string (AlwaysOn, AlwaysOff, 1~8) |
| Cockpit Sound | CockpitSoundData | intensity | Configures intensity for CockpitSoundData. | float |
| Control Base | ControlBaseData | attachPointId | Identifier/count related setting. | int |
| Control Base | ControlBaseData | axis | Configures axis for ControlBaseData. | Vector3(x,y,z) |
| Control Base | ControlBaseData | haptics | Configures haptics for ControlBaseData. | bool |
| Control Base | ControlBaseData | ignoreAircraftCollisions | Configures ignoreAircraftCollisions for ControlBaseData. | bool |
| Control Base | ControlBaseData | input | Configures input for ControlBaseData. | string |
| Control Base | ControlBaseData | max | Configures max for ControlBaseData. | float |
| Control Base | ControlBaseData | min | Configures min for ControlBaseData. | float |
| Control Base | ControlBaseData | mode | Mode/style selection setting. | Enum(ControlMode: Joint, Transform) |
| Control Base | ControlBaseData | name | Naming/text/interaction display setting. | string |
| Control Base | ControlBaseData | positionDamper | Position/path/target related setting. | float |
| Control Base | ControlBaseData | positionMaximumForce | Position/path/target related setting. | float |
| Control Base | ControlBaseData | positionSpring | Position/path/target related setting. | float |
| Control Base | ControlBaseData | rotationMaxDistance | Rotation/angle related setting. | float |
| Control Base | ControlBaseData | scale | Size/scale related setting. | float |
| Control Base | ControlBaseData | slerpDamper | Power/aerodynamics/physics parameter. | float |
| Control Base | ControlBaseData | slerpMaximumForce | Speed or timing related setting. | float |
| Control Base | ControlBaseData | slerpSpring | Power/aerodynamics/physics parameter. | float |
| Control Base | ControlBaseData | targetTransformPath | Position/path/target related setting. | string |
| Control Base | ControlBaseData | v | Configures v for ControlBaseData. | int |
| Control Surface | ControlSurfacePartData | dummyPartFlipped | Configures dummyPartFlipped for ControlSurfacePartData. | bool |
| Control Surface | ControlSurfacePartData | dummyWingOffset | Position/path/target related setting. | Vector2(x,y) |
| Control Surface | ControlSurfacePartData | dummyWingScale | Size/scale related setting. | Vector2(x,y) |
| Control Surface | ControlSurfacePartData | style | Mode/style selection setting. | string |
| Countermeasure Dispenser | CounterMeasureDispenserData | activationGroup | Activation group setting for grouped key/control triggering. | int |
| Countermeasure Dispenser | CounterMeasureDispenserData | ammo | Configures ammo for CounterMeasureDispenserData. | int |
| Countermeasure Dispenser | CounterMeasureDispenserData | autoDispenseDelay | Speed or timing related setting. | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | breakLockChance | Configures breakLockChance for CounterMeasureDispenserData. | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | evadeLockChance | Configures evadeLockChance for CounterMeasureDispenserData. | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | launchForce | Configures launchForce for CounterMeasureDispenserData. | float |
| Countermeasure Dispenser | CounterMeasureDispenserData | type | Mode/style selection setting. | Enum(CounterMeasureType: None, Flares, Chaff) |
| Decal | DecalData | color | Configures color for DecalData. | Color(HEX RGB) |
| Decal | DecalData | decalRotation | Rotation/angle related setting. | Vector3(x,y,z) |
| Decal | DecalData | opacity | Configures opacity for DecalData. | float |
| Decal | DecalData | partIds | Identifier/count related setting. | int list (comma separated) |
| Decal | DecalData | penetration | Configures penetration for DecalData. | float |
| Decal | DecalData | priority | Configures priority for DecalData. | int |
| Decal | DecalData | size | Size/scale related setting. | Vector3(x,y,z) |
| Decal | DecalData | target | Position/path/target related setting. | string (Single Part/MultipleParts) |
| Decal | TextureDecalData | decalId | Identifier/count related setting. | string |
| Decal | TextureDecalData | offset | Position/path/target related setting. | Vector2(x,y) |
| Decal | TextureDecalData | tiling | Configures tiling for TextureDecalData. | Vector2(x,y) |
| Detacher | DetacherData | attachPointsToDetach | Configures attachPointsToDetach for DetacherData. | int list (comma separated) |
| Detacher | DetacherData | delay | Speed or timing related setting. | float |
| Detacher | DetacherData | detacherUiMaxForce | Configures detacherUiMaxForce for DetacherData. | float |
| Detacher | DetacherData | detachForce | Configures detachForce for DetacherData. | float |
| Detacher | DetacherData | direction | Configures direction for DetacherData. | Enum(DetacherDirection: Default, Forward) |
| Detacher | DetacherData | enabled | Configures enabled for DetacherData. | bool |
| Detacher | DetacherData | group | Configures group for DetacherData. | string (0/1~8,0=Disabled) |
| Differential | JDifferentialData | coastStiffness | Configures coastStiffness for JDifferentialData. | float |
| Differential | JDifferentialData | lock | Configures lock for JDifferentialData. | float |
| Differential | JDifferentialData | powerStiffness | Power/aerodynamics/physics parameter. | float |
| Differential | JDifferentialData | size | Size/scale related setting. | float |
| Drive Shaft | JDriveHubData | reversed | Configures reversed for JDriveHubData. | bool |
| Drive Shaft | JDriveShaftData | bootA | Configures bootA for JDriveShaftData. | bool |
| Drive Shaft | JDriveShaftData | bootB | Configures bootB for JDriveShaftData. | bool |
| Drive Shaft | JDriveShaftData | end | Configures end for JDriveShaftData. | Vector3(x,y,z) |
| Drive Shaft | JDriveShaftData | radius | Size/scale related setting. | float |
| Drive Shaft | JDriveShaftData | start | Configures start for JDriveShaftData. | Vector3(x,y,z) |
| Drive Shaft | JDriveShaftData | visual | Configures visual for JDriveShaftData. | bool |
| Engine | EngineData | alphaTiedToThrottle | Configures alphaTiedToThrottle for EngineData. | bool |
| Engine | EngineData | ductedThrust | Power/aerodynamics/physics parameter. | bool |
| Engine | EngineData | exhaustScale | Size/scale related setting. | Vector3(x,y,z) |
| Engine | EngineData | fuelConsumptionRate | Speed or timing related setting. | float |
| Engine | EngineData | power | Power/aerodynamics/physics parameter. | float |
| Engine | EngineData | powerMultiplier | Power/aerodynamics/physics parameter. | float |
| Engine | EngineData | requiredAirIntake | Configures requiredAirIntake for EngineData. | float |
| Engine | EngineData | soundOverride | Identifier/count related setting. | string |
| Engine | EngineData | throttleResponse | Configures throttleResponse for EngineData. | float |
| Engine | EngineData | type | Mode/style selection setting. | Enum(EngineType: Prop, Turbojet, AfterburningTurbojet) |
| Engine | JEngineData | basePower | Power/aerodynamics/physics parameter. | float |
| Engine | JEngineData | baseRpm | Speed or timing related setting. | float |
| Engine | JEngineData | baseSize | Size/scale related setting. | float |
| Engine | JEngineData | cylinderRows | Configures cylinderRows for JEngineData. | int |
| Engine | JEngineData | engineConfiguration | Configures engineConfiguration for JEngineData. | int |
| Engine | JEngineData | engineTuning | Configures engineTuning for JEngineData. | float |
| Engine | JEngineData | forcedInduction | Configures forcedInduction for JEngineData. | float |
| Engine | JEngineData | horsePower | Power/aerodynamics/physics parameter. | float |
| Engine | JEngineData | mass | Configures mass for JEngineData. | float |
| Engine | JEngineData | massToPower | Power/aerodynamics/physics parameter. | float |
| Engine | JEngineData | powerCurve | Power/aerodynamics/physics parameter. | string |
| Engine | JEngineData | redLine | Configures redLine for JEngineData. | float |
| Engine | JEngineData | rpm | Speed or timing related setting. | float |
| Engine | JEngineData | rpmScalingExponent | Speed or timing related setting. | float |
| Engine | JEngineData | size | Size/scale related setting. | float |
| Engine | JEngineData | soundPitchLimit | Configures soundPitchLimit for JEngineData. | float |
| Engine | JEngineData | soundPitchOffset | Position/path/target related setting. | float |
| Engine | JEngineData | soundPitchRange | Configures soundPitchRange for JEngineData. | float |
| Engine | JEngineData | soundType | Mode/style selection setting. | Enum(EngineSoundType: None, Prop, Car, Boat, V, Flat, Radial, Inline, Electric, PropV, PropFlat, PropRadial, CarV, CarFlat, CarInline) |
| Engine | JEngineData | startupDuration | Speed or timing related setting. | float |
| Engine | JEngineData | supercharger | Configures supercharger for JEngineData. | bool |
| Engine | JEngineData | superchargerMultiplier | Configures superchargerMultiplier for JEngineData. | float |
| Engine | JEngineData | throttleResponse | Configures throttleResponse for JEngineData. | float |
| Floating Part | FloatingPartData | enabled | Configures enabled for FloatingPartData. | bool |
| Floating Part | FloatingPartData | impactVelocityAdjustment | Configures impactVelocityAdjustment for FloatingPartData. | string (curve nameorsingle float value) |
| Floating Part | FloatingPartData | reduceBuoyancyIfBySelf | Configures reduceBuoyancyIfBySelf for FloatingPartData. | bool |
| Floating Part | FloatingPartData | weightFactor | Configures weightFactor for FloatingPartData. | float |
| Fuel Tank | FuelTankData | capacity | Configures capacity for FuelTankData. | float |
| Fuel Tank | FuelTankData | fuel | Power/aerodynamics/physics parameter. | float |
| Fuel Tank | ResizableFuelTankData | capacity | Configures capacity for ResizableFuelTankData. | float |
| Fuel Tank | ResizableFuelTankData | size | Size/scale related setting. | float |
| Fuselage | FuselageData | autoSizeOnConnected | Size/scale related setting. | bool |
| Fuselage | FuselageData | buoyancy | Configures buoyancy for FuselageData. | float |
| Fuselage | FuselageData | collider | Identifier/count related setting. | Enum(FuselageColliderType: Auto, Basic, ConvexMesh, NonConvexMesh) |
| Fuselage | FuselageData | collider | Identifier/count related setting. | Enum(FuselageData.FuselageColliderType: Auto, Basic, ConvexMesh, NonConvexMesh) |
| Fuselage | FuselageData | cornerTypes | Mode/style selection setting. | int list (8 items,comma separated) |
| Fuselage | FuselageData | deadWeight | Configures deadWeight for FuselageData. | float |
| Fuselage | FuselageData | fillBack | Configures fillBack for FuselageData. | float or float4(top,bottom,left,right) |
| Fuselage | FuselageData | fillCutFace | Configures fillCutFace for FuselageData. | bool |
| Fuselage | FuselageData | fillFront | Configures fillFront for FuselageData. | float or float4(top,bottom,left,right) |
| Fuselage | FuselageData | frontScale | Size/scale related setting. | Vector2(x,y) |
| Fuselage | FuselageData | fuelPercentage | Power/aerodynamics/physics parameter. | float |
| Fuselage | FuselageData | inletSlant | Configures inletSlant for FuselageData. | float |
| Fuselage | FuselageData | inletThicknessFront | Size/scale related setting. | float |
| Fuselage | FuselageData | inletThicknessRear | Size/scale related setting. | float |
| Fuselage | FuselageData | inletTrimSize | Size/scale related setting. | float |
| Fuselage | FuselageData | offset | Position/path/target related setting. | Vector3(x,y,z) |
| Fuselage | FuselageData | rearScale | Size/scale related setting. | Vector2(x,y) |
| Fuselage | FuselageData | smoothBack | Configures smoothBack for FuselageData. | bool |
| Fuselage | FuselageData | smoothFront | Configures smoothFront for FuselageData. | bool |
| Fuselage | FuselageData | type | Mode/style selection setting. | string (body, cone, inlet, hollow, glass, hollowglass) |
| Fuselage | FuselageData | version | Configures version for FuselageData. | int |
| Fuselage | JFuselageData | autoResize | Size/scale related setting. | bool |
| Fuselage | JFuselageData | buoyancy | Configures buoyancy for JFuselageData. | float |
| Fuselage | JFuselageData | colliderCornerSamples | Identifier/count related setting. | int |
| Fuselage | JFuselageData | cornerRadii | Configures cornerRadii for JFuselageData. | Vector4(x,y,z,w) |
| Fuselage | JFuselageData | cornerSamples | Configures cornerSamples for JFuselageData. | Int4(x,y,z,w) |
| Fuselage | JFuselageData | cornerStretch | Configures cornerStretch for JFuselageData. | Bool4(x,y,z,w) |
| Fuselage | JFuselageData | cutting | Configures cutting for JFuselageData. | decimal?list (4 items,comma separated,optional blank) |
| Fuselage | JFuselageData | deadMassKg | Configures deadMassKg for JFuselageData. | float |
| Fuselage | JFuselageData | defaultThicknessFront | Size/scale related setting. | float |
| Fuselage | JFuselageData | defaultThicknessRear | Size/scale related setting. | float |
| Fuselage | JFuselageData | edgeCurvature | Configures edgeCurvature for JFuselageData. | Vector4(x,y,z,w) |
| Fuselage | JFuselageData | edgeSamples | Configures edgeSamples for JFuselageData. | Int4(x,y,z,w) |
| Fuselage | JFuselageData | fuelProportion | Power/aerodynamics/physics parameter. | float |
| Fuselage | JFuselageData | glass | Configures glass for JFuselageData. | bool |
| Fuselage | JFuselageData | legacyThickness | Size/scale related setting. | bool |
| Fuselage | JFuselageData | mass | Configures mass for JFuselageData. | Vector4(x,y,z,w) |
| Fuselage | JFuselageData | noseconeRoundness | Configures noseconeRoundness for JFuselageData. | float |
| Fuselage | JFuselageData | numColliders | Identifier/count related setting. | int |
| Fuselage | JFuselageData | offset | Position/path/target related setting. | Vector3(x,y,z) |
| Fuselage | JFuselageData | size | Size/scale related setting. | Vector2(x,y) |
| Fuselage | JFuselageData | smoothing | Configures smoothing for JFuselageData. | bool |
| Fuselage | JFuselageData | style | Mode/style selection setting. | Enum(FuselageStyle: Body, Hollow, Inlet, Cone, HollowCone) |
| Fuselage | JFuselageData | syncSlices | Configures syncSlices for JFuselageData. | bool |
| Fuselage | JFuselageData | thickness | Size/scale related setting. | float |
| Fuselage | JFuselageData | trapezium | Configures trapezium for JFuselageData. | float |
| Fuselage | JFuselageData | version | Configures version for JFuselageData. | int |
| Gauge | GaugeData | altitudeUnit | Configures altitudeUnit for GaugeData. | Enum(GaugeData.AltitudeUnit: Feet, Meters, None) |
| Gauge | GaugeData | face | Configures face for GaugeData. | Enum(GaugeData.GaugeFaceTypes: AirSpeed200Indicator, AirSpeed400Indicator, AirSpeed600Indicator, AltimeterIndicator, AttitudeIndicator, FuelIndicator, HeadingIndicator, ThrottleIndicator, TrimIndicator, TurnCoordinatorIndicator, VerticalSpeedIndicator, VTOLIndicator, RotorRPM, Basic1) |
| Gauge | GaugeData | faceEmission | Configures faceEmission for GaugeData. | float |
| Gauge | GaugeData | faceEmissionDay | Configures faceEmissionDay for GaugeData. | float |
| Gauge | GaugeData | faceEmissionNight | Configures faceEmissionNight for GaugeData. | float |
| Gauge | GaugeData | faceInput | Configures faceInput for GaugeData. | string |
| Gauge | GaugeData | faceMultiplier | Configures faceMultiplier for GaugeData. | float |
| Gauge | GaugeData | faceZero | Configures faceZero for GaugeData. | float |
| Gauge | GaugeData | hideBase | Identifier/count related setting. | bool |
| Gauge | GaugeData | hideFace | Identifier/count related setting. | bool |
| Gauge | GaugeData | hideTrim | Identifier/count related setting. | bool |
| Gauge | GaugeData | indicator | Configures indicator for GaugeData. | Enum(GaugeData.IndicatorType: Indicator1, Indicator2, Indicator3, Indicator4, Indicator5, Indicator6, Indicator7, None) |
| Gauge | GaugeData | indicatorZero | Configures indicatorZero for GaugeData. | float |
| Gauge | GaugeData | input | Configures input for GaugeData. | string |
| Gauge | GaugeData | invert | Configures invert for GaugeData. | bool |
| Gauge | GaugeData | multiplier | Configures multiplier for GaugeData. | float |
| Gauge | GaugeData | rotationType | Rotation/angle related setting. | Enum(GaugeData.GaugeRotationType: Indicator, Face) |
| Gauge | GaugeData | scale | Size/scale related setting. | float |
| Gauge | GaugeData | speedUnit | Speed or timing related setting. | Enum(GaugeData.SpeedUnit: Knots, MetersPerSecond, MilesPerHour, KilometersPerHour, None) |
| Gauge | GaugeData | trimType | Mode/style selection setting. | Enum(GaugeData.GaugeTrimType: Trim1, Trim2) |
| Gauge | GaugeData | type | Mode/style selection setting. | Enum(GaugeData.GaugeTypePreset: Custom, Heading, Fuel, Throttle, Speed200, Speed400, Speed600, Altitude, Trim, TurnCoordinator, VerticalSpeed, RotorRPM, VTOL, BankAngle) |
| Gauge | GaugeData | zero | Configures zero for GaugeData. | float |
| Gearbox | JGearboxData | gearRatio | Configures gearRatio for JGearboxData. | float |
| Gearbox | JGearboxData | reversed | Configures reversed for JGearboxData. | bool |
| Gearbox | JGearboxData | size | Size/scale related setting. | float |
| Gun | GunData | activationGroup | Activation group setting for grouped key/control triggering. | string (All, 1~8) |
| Gun | GunData | ammoCount | Identifier/count related setting. | int |
| Gun | GunData | bulletScale | Size/scale related setting. | Vector3(x,y,z) |
| Gun | GunData | burstCount | Identifier/count related setting. | int |
| Gun | GunData | damage | Configures damage for GunData. | float |
| Gun | GunData | impactForce | Configures impactForce for GunData. | float |
| Gun | GunData | lifetime | Configures lifetime for GunData. | float |
| Gun | GunData | muzzleFlash | Configures muzzleFlash for GunData. | bool |
| Gun | GunData | muzzleVelocity | Configures muzzleVelocity for GunData. | float |
| Gun | GunData | roundsPerSecond | Configures roundsPerSecond for GunData. | float |
| Gun | GunData | spread | Configures spread for GunData. | float |
| Gun | GunData | timeBetweenBursts | Configures timeBetweenBursts for GunData. | float |
| Gun | GunData | tracerIntensity | Configures tracerIntensity for GunData. | float |
| Gyroscope | GyroscopeData | activationGroup | Activation group setting for grouped key/control triggering. | string (None, 1~8) |
| Gyroscope | GyroscopeData | autoOrient | Configures autoOrient for GyroscopeData. | bool |
| Gyroscope | GyroscopeData | pitchRange | Configures pitchRange for GyroscopeData. | float |
| Gyroscope | GyroscopeData | rollRange | Configures rollRange for GyroscopeData. | float |
| Gyroscope | GyroscopeData | speed | Speed or timing related setting. | float |
| Gyroscope | GyroscopeData | stability | Configures stability for GyroscopeData. | float |
| Gyroscope | GyroscopeData | yawPower | Power/aerodynamics/physics parameter. | float |
| IK Target | IKTargetData | offset | Position/path/target related setting. | Vector3(x,y,z) |
| IK Target | IKTargetData | path | Position/path/target related setting. | string |
| IK Target | IKTargetData | positionWeight | Position/path/target related setting. | float |
| IK Target | IKTargetData | priority | Configures priority for IKTargetData. | int |
| IK Target | IKTargetData | rotationWeight | Rotation/angle related setting. | float |
| IK Target | IKTargetData | type | Mode/style selection setting. | Enum(IKTargetType: Body, LeftShoulder, RightShoulder, LeftThigh, RightThigh, LeftHand, RightHand, LeftFoot, RightFoot, LeftElbow, RightElbow, LeftKnee, RightKnee) |
| Inlet | InletData | airIntakeMultiplier | Configures airIntakeMultiplier for InletData. | float |
| Input Controller | InputControllerData | activationGroup | Activation group setting for grouped key/control triggering. | string (0~8) |
| Input Controller | InputControllerData | defaultActivationGroup | Activation group setting for grouped key/control triggering. | string (0~8) |
| Input Controller | InputControllerData | defaultInput | Configures defaultInput for InputControllerData. | string |
| Input Controller | InputControllerData | defaultMax | Configures defaultMax for InputControllerData. | float |
| Input Controller | InputControllerData | defaultMin | Configures defaultMin for InputControllerData. | float |
| Input Controller | InputControllerData | input | Configures input for InputControllerData. | string |
| Input Controller | InputControllerData | invert | Configures invert for InputControllerData. | bool |
| Input Controller | InputControllerData | invertOnMirror | Configures invertOnMirror for InputControllerData. | bool |
| Input Controller | InputControllerData | invertType | Mode/style selection setting. | Enum(InvertType: Axis, Output) |
| Input Controller | InputControllerData | max | Configures max for InputControllerData. | float |
| Input Controller | InputControllerData | min | Configures min for InputControllerData. | float |
| Input Controller | InputControllerData | name | Naming/text/interaction display setting. | string |
| Input Controller | InputControllerData | propertyEditorDesc | Configures propertyEditorDesc for InputControllerData. | string |
| Input Controller | InputControllerData | zeroOnDeactivate | Configures zeroOnDeactivate for InputControllerData. | bool |
| Jet Engine | JetEngineData | afterburner | Power/aerodynamics/physics parameter. | bool |
| Jet Engine | JetEngineData | afterburnerBaseColor | Power/aerodynamics/physics parameter. | Color(HTML Hex RGBA) |
| Jet Engine | JetEngineData | afterburnerThrottleStart | Power/aerodynamics/physics parameter. | float |
| Jet Engine | JetEngineData | afterburnerTipColor | Power/aerodynamics/physics parameter. | Color(HTML Hex RGBA) |
| Jet Engine | JetEngineData | baseSize | Size/scale related setting. | float |
| Jet Engine | JetEngineData | burnerTemp | Power/aerodynamics/physics parameter. | float |
| Jet Engine | JetEngineData | burnerTempRange | Power/aerodynamics/physics parameter. | float list (2 items: min,max) |
| Jet Engine | JetEngineData | bypassRange | Configures bypassRange for JetEngineData. | float list (2 items: min,max) |
| Jet Engine | JetEngineData | bypassRatio | Configures bypassRatio for JetEngineData. | float |
| Jet Engine | JetEngineData | compressionRange | Configures compressionRange for JetEngineData. | float list (2 items: min,max) |
| Jet Engine | JetEngineData | compressionRatio | Configures compressionRatio for JetEngineData. | float |
| Jet Engine | JetEngineData | coreVisualScale | Size/scale related setting. | float |
| Jet Engine | JetEngineData | fanPressureRatio | Configures fanPressureRatio for JetEngineData. | float |
| Jet Engine | JetEngineData | fanStyle | Mode/style selection setting. | string |
| Jet Engine | JetEngineData | gimbalSpeed | Speed or timing related setting. | float |
| Jet Engine | JetEngineData | inletConeStyle | Mode/style selection setting. | string |
| Jet Engine | JetEngineData | jetEngineType | Mode/style selection setting. | Enum(JetEngineType: None, Legacy, Civilian, Military) |
| Jet Engine | JetEngineData | mass | Configures mass for JetEngineData. | float |
| Jet Engine | JetEngineData | maxGimbalAngle | Rotation/angle related setting. | float |
| Jet Engine | JetEngineData | nozzleLength | Size/scale related setting. | float |
| Jet Engine | JetEngineData | nozzleStyle | Mode/style selection setting. | string |
| Jet Engine | JetEngineData | reverseThrust | Power/aerodynamics/physics parameter. | bool |
| Jet Engine | JetEngineData | size | Size/scale related setting. | float |
| Jet Engine | JetEngineData | sizeRange | Size/scale related setting. | float list (2 items: min,max) |
| Jet Engine | JetEngineData | turbinePressureRatio | Configures turbinePressureRatio for JetEngineData. | float |
| Jet Engine Shroud | JetEngineShroudData | jetEngineType | Mode/style selection setting. | Enum(JetEngineType: None, Legacy, Civilian, Military) |
| Jet Engine Shroud | JetEngineShroudData | length | Size/scale related setting. | float |
| Jet Engine Shroud | JetEngineShroudData | radius | Size/scale related setting. | float |
| Jet Engine Shroud | JetEngineShroudData | style | Mode/style selection setting. | string |
| Joint Motor | JointMotorData | attachPoint | Configures attachPoint for JointMotorData. | int |
| Joystick | AdjustableJoystickData | colliderPath | Position/path/target related setting. | string |
| Joystick | AdjustableJoystickData | cylinderPath | Position/path/target related setting. | string |
| Joystick | AdjustableJoystickData | headPaths | Position/path/target related setting. | string list (comma separated node paths) |
| Joystick | AdjustableJoystickData | height | Configures height for AdjustableJoystickData. | float |
| Label | LabelData | curvature | Configures curvature for LabelData. | float |
| Label | LabelData | curvatureDirection | Configures curvatureDirection for LabelData. | Enum(LabelCurvatureDirection: Horizontal, Vertical) |
| Label | LabelData | designText | Naming/text/interaction display setting. | string |
| Label | LabelData | emission | Configures emission for LabelData. | float |
| Label | LabelData | emissionDay | Configures emissionDay for LabelData. | float |
| Label | LabelData | emissionNight | Configures emissionNight for LabelData. | float |
| Label | LabelData | fontName | Mode/style selection setting. | string |
| Label | LabelData | fontSize | Size/scale related setting. | float |
| Label | LabelData | gradient | Configures gradient for LabelData. | Enum(LabelPartGradientType: None, Vertical, Horizontal, Diagonal, UpperLeft, UpperRight, LowerLeft, LowerRight) |
| Label | LabelData | height | Configures height for LabelData. | float |
| Label | LabelData | horizontalAlignment | Mode/style selection setting. | Enum(Left, Center, Right) |
| Label | LabelData | offset | Position/path/target related setting. | Vector3(x,y,z) |
| Label | LabelData | outlineWidth | Size/scale related setting. | float |
| Label | LabelData | paintIndexShift | Configures paintIndexShift for LabelData. | int |
| Label | LabelData | parentPath | Position/path/target related setting. | string |
| Label | LabelData | renderQueueOffset | Position/path/target related setting. | int |
| Label | LabelData | supportsCurvature | Configures supportsCurvature for LabelData. | bool |
| Label | LabelData | supportsGradient | Configures supportsGradient for LabelData. | bool |
| Label | LabelData | verticalAlignment | Mode/style selection setting. | Enum(Top, Middle, Bottom) |
| Label | LabelData | width | Size/scale related setting. | float |
| Landing Gear | RetractableLandingGearData | (none) | This part reads no unique attribute in its own state; behavior mainly comes from base/shared logic. | None |
| Landing Gear | WheelData | (none) | This part reads no unique attribute in its own state; behavior mainly comes from base/shared logic. | None |
| Landing Gear | WingLandingGearData | (none) | This part reads no unique attribute in its own state; behavior mainly comes from base/shared logic. | None |
| Magnet | MagnetData | activationGroup | Activation group setting for grouped key/control triggering. | string (None, 1~8) |
| Magnet | MagnetData | power | Power/aerodynamics/physics parameter. | float |
| Main Rotor | HeliMainRotorData | centerOfMassOffset | Position/path/target related setting. | Vector3(x,y,z) |
| Main Rotor | HeliMainRotorData | cyclicPitchMaxDeflection | Configures cyclicPitchMaxDeflection for HeliMainRotorData. | float |
| Main Rotor | HeliMainRotorData | cyclicRollMaxDeflection | Configures cyclicRollMaxDeflection for HeliMainRotorData. | float |
| Main Rotor | HeliMainRotorData | rotorDamping | Configures rotorDamping for HeliMainRotorData. | float |
| MFD | MfdData | targetingPod | Position/path/target related setting. | int (target part ID) |
| Missile | MissileData | function | Configures function for MissileData. | Enum(WeaponFunction: None, AirToAir, AirToSurface, MultiRole) |
| Missile | MissileData | guidanceActivationDelay | Speed or timing related setting. | float |
| Missile | MissileData | ignitionDelay | Speed or timing related setting. | float |
| Missile | MissileData | killCam | Configures killCam for MissileData. | bool |
| Missile | MissileData | loft | Configures loft for MissileData. | float |
| Missile | MissileData | maxForwardThrustForce | Power/aerodynamics/physics parameter. | float |
| Missile | MissileData | maxFuelTime | Power/aerodynamics/physics parameter. | float |
| Missile | MissileData | maxHeadingAngleAdjustmentRate | Rotation/angle related setting. | float |
| Missile | MissileData | maxRange | Configures maxRange for MissileData. | float |
| Missile | MissileData | maxSpeed | Speed or timing related setting. | float |
| Missile | MissileData | maxTargetingAngle | Position/path/target related setting. | float |
| Missile | MissileData | maxThrustVectoringRate | Speed or timing related setting. | float |
| Missile | MissileData | maxTorque | Power/aerodynamics/physics parameter. | float |
| Missile | MissileData | maxVelocityAngleAdjustmentRate | Rotation/angle related setting. | float |
| Missile | MissileData | minRange | Configures minRange for MissileData. | float |
| Missile | MissileData | proximityDetonationRangeMax | Configures proximityDetonationRangeMax for MissileData. | float |
| Missile | MissileData | proximityDetonationRangeMin | Configures proximityDetonationRangeMin for MissileData. | float |
| Missile | MissileData | seeker | Configures seeker for MissileData. | Enum(SeekerType: Unguided, Infrared, SemiActiveRadar, ActiveRadar, Laser, AntiRadiation) |
| Missile | MissileData | smokeOpacity | Configures smokeOpacity for MissileData. | float |
| Missile | MissileData | smokeScale | Size/scale related setting. | float |
| Missile | MissileData | waterproof | Configures waterproof for MissileData. | bool |
| Missile Configuration | ProceduralMissileData | attachPosition | Position/path/target related setting. | float (-1~1) |
| Missile Configuration | ProceduralMissileData | body | Configures body for ProceduralMissileData. | string |
| Missile Configuration | ProceduralMissileData | burnTime | Power/aerodynamics/physics parameter. | float (0~1) |
| Missile Configuration | ProceduralMissileData | engine | Configures engine for ProceduralMissileData. | Enum(MissileEngineType: Solid, ThrustVector, Jet) |
| Missile Configuration | ProceduralMissileData | nose | Configures nose for ProceduralMissileData. | string |
| Missile Configuration | ProceduralMissileData | noseLength | Missile nose length. | float |
| Missile Configuration | ProceduralMissileData | radius | Size/scale related setting. | float |
| Missile Configuration | ProceduralMissileData | seeker | Seeker type configuration. | Enum(SeekerType: Unguided, Infrared, SemiActiveRadar, ActiveRadar, Laser, AntiRadiation) |
| Missile Configuration | ProceduralMissileData | seekerFOV | Seeker field-of-view angle. | float |
| Missile Configuration | ProceduralMissileData | size | Size/scale related setting. | float |
| Missile Configuration | ProceduralMissileData | updateMissileModifier | Refresh missile modifier after parameter changes. | bool |
| Missile Configuration | ProceduralMissileData | warheadBias | Warhead bias/placement parameter. | float |
| Nosecone | AdaptiveNoseConeData | scale | Size/scale related setting. | Vector3(x,y,z) |
| Parachute | ParachuteData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Parachute | ParachuteData | size | Size/scale related setting. | float |
| Parachute | ParachuteData | style | Mode/style selector. | string |
| Part Targeting | PartTargetingData | customPartIds | Custom target part ID list. | int list (comma separated) |
| Part Targeting | PartTargetingData | partIds | Referenced part ID list. | int list (comma separated) |
| Part Targeting | PartTargetingData | targetMode | Part targeting mode. | Enum(PartTargetingMode: SinglePart, MultipleParts, Custom) |
| Pedal | PedalData | fullAngle | Full travel angle. | float |
| Pedal | PedalData | input | Configures input for Pedal. | string |
| Pedal | PedalData | zeroAngle | Zero position angle. | float |
| Piston | PistonData | attachPoint | Configures attachPoint for Piston. | int |
| Piston | PistonData | cycle | Configures cycle for Piston. | bool |
| Piston | PistonData | extend | Configures extend for Piston. | bool |
| Piston | PistonData | maxRange | Maximum range value. | float |
| Piston | PistonData | maxSpeed | Maximum speed limit. | float |
| Piston | PistonData | preventBreaking | Configures preventBreaking for Piston. | bool |
| Piston | PistonData | range | Operational range/travel. | float |
| Piston | PistonData | speed | Speed/time process setting. | float |
| Posed Grip | PosedGripData | asButton | Treat input as button mode. | bool |
| Posed Grip | PosedGripData | colliders | Collider path list (comma separated). | string |
| Posed Grip | PosedGripData | control | Control binding name. | string |
| Posed Grip | PosedGripData | controlPath | XR control path. | string |
| Posed Grip | PosedGripData | disableTooltip | Disable tooltip display. | bool |
| Posed Grip | PosedGripData | gripTarget | Grip target transform path. | string |
| Posed Grip | PosedGripData | gripType | XR grip control scheme (ungripped / primary / secondary). | Enum(XRControlGripType: Default/FlightStick/Throttle) |
| Posed Grip | PosedGripData | outlineScale | Size/scale related setting. | Vector3(x,y,z) |
| Posed Grip | PosedGripData | pose | Grip pose name. | string |
| Posed Grip | PosedGripData | previewPose | Preview pose in editor. | string |
| Posed Grip | PosedGripData | processor | Input processor expression. | string |
| Posed Grip | PosedGripData | tooltip | Tooltip text. | string |
| Posed Grip | PosedGripData | tooltipOffset | Tooltip offset value. | float |
| Posed Grip | PosedGripData | tooltipTransformPath | Tooltip anchor transform path. | string |
| Procedural Bay | ProceduralBayData | doorStyle | Door opening style. | Enum(DoorStyle: None, SingleLeft, SingleRight, Double) |
| Procedural Bay | ProceduralBayData | startOpen | Whether the part starts open. | bool |
| Procedural Window | ProceduralWindowData | hideGlass | Hide glass layer. | bool |
| Propeller Engine | PropEngineAdvancedData | legacyCotPos | Use legacy center-of-thrust position logic. | bool |
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
| Propellers | PropellerAssemblyData | pushProp | Use pusher configuration. | bool |
| Propellers | PropellerAssemblyData | reverseBladeDirection | Reverse blade rotation direction. | bool |
| Propellers | PropellerAssemblyData | size | Size/scale related setting. | float |
| Propellers | PropellerAssemblyData | thrustScalar | Thrust scale factor. | float |
| Propellers | PropellerAssemblyData | twistAngleRoot | Root blade twist angle. | float |
| Reaction Control Nozzle | ReactionControlNozzleData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Reaction Control Nozzle | ReactionControlNozzleData | autoAssignType | Auto-detect axis type for nozzle control. | bool |
| Reaction Control Nozzle | ReactionControlNozzleData | fuelConsumptionRate | Fuel consumption rate. | float |
| Reaction Control Nozzle | ReactionControlNozzleData | power | Power/strength output parameter. | float |
| Reaction Control Nozzle | ReactionControlNozzleData | reverse | Reverse output direction. | bool |
| Reaction Control Nozzle | ReactionControlNozzleData | type | RCS nozzle axis type (pitch / roll / yaw). | Enum(ReactionControlNozzleType: Pitch/Roll/Yaw) |
| Refuel Drouge | RefuelDrogueData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Refuel Drouge | RefuelDrogueData | angularDragPower | Angular drag strength. | float |
| Refuel Drouge | RefuelDrogueData | angularStabPower | Angular stabilization strength. | float |
| Refuel Drouge | RefuelDrogueData | transferRate | Transfer rate. | float |
| Refuel Drouge | RefuelDrogueData | triggerColliderPath | Trigger collider path. | string |
| Refuel Probe | RefuelProbeData | offset | Position/path/target related setting. | Vector2(x,y) |
| Resizable Shape | ResizableShapeData | attachPointPosition | Attach point position. | Vector3(x,y,z) |
| Resizable Shape | ResizableShapeData | bounciness | Bounciness coefficient. | float |
| Resizable Shape | ResizableShapeData | friction | Friction coefficient. | float |
| Resizable Shape | ResizableShapeData | size | Raw size value of resizable sphere; runtime visual radius equals value/4. | float (runtime radius = value/4) |
| Rocket | RocketWeaponData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Rocket | RocketWeaponData | burnTimer | Burn timer setting. | float |
| Rocket | RocketWeaponData | explosionScale | Explosion scale factor. | float |
| Rocket | RocketWeaponData | finMode | Fin mode/config marker. | string |
| Rocket | RocketWeaponData | firingDelay | Firing delay. | float |
| Rocket | RocketWeaponData | laserGuided | Enable laser guidance. | bool |
| Rocket | RocketWeaponData | name | Naming/text/interaction display setting. | string |
| Rocket | RocketWeaponData | selfDestructTimer | Self-destruct timer. | float |
| Rocket Pod | RocketPodData | activationGroup | Activation group index used to trigger the part with key groups. | string |
| Rocket Pod | RocketPodData | explosionScale | Explosion scale factor. | float |
| Rocket Pod | RocketPodData | firingDelay | Firing delay. | float |
| Rocket Pod | RocketPodData | laserGuided | Enable laser guidance. | bool |
| Rocket Pod | RocketPodData | name | Naming/text/interaction display setting. | string |
| Rotator | JointRotatorData | allowFreeSpin | Allow free spinning. | bool |
| Rotator | JointRotatorData | attachPoint | Configures attachPoint for Rotator. | int |
| Rotator | JointRotatorData | audio | Enable rotation audio. | bool |
| Rotator | JointRotatorData | damperMultiplier | Damper multiplier. | float |
| Rotator | JointRotatorData | disableBaseMesh | Hide base mesh. | bool |
| Rotator | JointRotatorData | hingeOffset | Hinge offset. | Vector3(x,y,z) |
| Rotator | JointRotatorData | maxRange | Maximum range value. | int |
| Rotator | JointRotatorData | maxSpeed | Maximum speed limit. | float |
| Rotator | JointRotatorData | minRange | Minimum range value. | int |
| Rotator | JointRotatorData | range | Operational range/travel. | float |
| Rotator | JointRotatorData | shortestAngle | Use shortest angle path for rotation. | bool |
| Rotator | JointRotatorData | speed | Speed/time process setting. | float |
| Rotator | JointRotatorData | supportsDisableBaseMesh | Supports hiding base mesh. | bool |
| Seat | SeatData | animation | Animation state/resource name. | string |
| Seat | SeatData | exitPosition | Exit position. | Vector3(x,y,z) |
| Seat | SeatData | exitRotation | Exit rotation. | Vector3(x,y,z) |
| Seat | SeatData | primarySeat | Whether this is the primary seat. | bool |
| Seat | SeatData | reclination | Seat recline amount. | float |
| Seat | SeatData | seatedPosition | Seated position. | Vector3(x,y,z) |
| Seat | SeatData | seatedRotation | Seated rotation. | Vector3(x,y,z) |
| Seat IK | IKSeatData | bodyTarget | Body IK target. | int |
| Seat IK | IKSeatData | designerCharacter | Designer character id. | string |
| Seat IK | IKSeatData | fpvTracking | Enable first-person tracking. | bool |
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
| Seat IK | IKSeatData | selfAssignTargets | Auto assign IK targets. | bool |
| Seat IK | IKSeatData | snapRange | IK snap range. | float |
| Suspension | SuspensionData | attachPoint | Configures attachPoint for Suspension. | int |
| Suspension | SuspensionData | damper | Damping factor. | float |
| Suspension | SuspensionData | spring | Spring stiffness. | float |
| Switch | CockpitSwitchData | angleOff | Off-state angle. | float |
| Switch | CockpitSwitchData | angleOn | On-state angle. | float |
| Switch | CockpitSwitchData | axis | Axis mapping. | Vector3(x,y,z) |
| Switch | CockpitSwitchData | disableTooltip | Disable tooltip display. | bool |
| Switch | CockpitSwitchData | inputId | Input identifier. | string |
| Switch | CockpitSwitchData | outputValue | Output value. | float |
| Switch | CockpitSwitchData | positionTransitionDelay | Position transition delay. | float |
| Switch | CockpitSwitchData | positionTransitionTime | Position transition duration. | float |
| Switch | CockpitSwitchData | scale | Size/scale related setting. | float |
| Switch | CockpitSwitchData | style | Mode/style selector. | Enum(CockpitSwitchData.CockpitSwitchStyle: Default, Flip, Rocker, Pivot) |
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
| Targeting Pod | TargetingPodData | offset | Position/path/target related setting. | Vector3(x,y,z) |
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
| Transmission | JTransmissionData | size | Size/scale related setting. | float |
| Transmission | JTransmissionData | transmissionType | Transmission type. | Enum(JTransmissionData.JTransmissionType: Automatic, Manual) |
| Transmission | JTransmissionData | variableShift | Variable shift strategy parameter. | float |
| Transparency | TransparencyData | alwaysFindConnected | Always include connected parts when evaluating transparency. | bool |
| Transparency | TransparencyData | hideBack | Hide back faces. | bool |
| Transparency | TransparencyData | hideFront | Hide front faces. | bool |
| Transparency | TransparencyData | hideInside | Hide inside faces. | bool |
| Transparency | TransparencyData | opacity | Opacity value. | float |
| Transparency | TransparencyData | overrideHide | Override default hide behavior. | bool |
| Wheel | JWheelData | brake | Brake strength. | float |
| Wheel | JWheelData | duals | Dual wheel/tire setup. | bool |
| Wheel | JWheelData | forcePoint | Force application point parameter. | float |
| Wheel | JWheelData | frictionCirclePower | Friction circle power. | float |
| Wheel | JWheelData | frictionCircleStrength | Friction circle strength. | float |
| Wheel | JWheelData | frictionPreset | Friction preset id/name. | string |
| Wheel | JWheelData | hideRims | Hide rims. | bool |
| Wheel | JWheelData | magicEngineId | Linked engine identifier. | int |
| Wheel | JWheelData | reversed | Reverse wheel direction. | bool |
| Wheel | JWheelData | rim | Rim style. | string |
| Wheel | JWheelData | rimOffset | Rim offset. | float |
| Wheel | JWheelData | size | Size/scale related setting. | float |
| Wheel | JWheelData | tire | Tire style. | string |
| Wheel | JWheelData | tractionForward | Forward traction coefficient. | float |
| Wheel | JWheelData | tractionSideways | Sideways traction coefficient. | float |
| Wheel | JWheelData | turningAngle | Maximum steering angle. | float |
| Wheel | JWheelData | turningAngleDampening | Steering angle dampening. | float |
| Wheel | JWheelData | turningRate | Steering rate. | float |
| Wheel | JWheelData | width | Size/scale related setting. | float |
| Wheel | ResizableWheelData | brakeTorque | Brake torque. | float |
| Wheel | ResizableWheelData | damper | Damping factor. | float |
| Wheel | ResizableWheelData | direction | Drive/rotation direction. | string |
| Wheel | ResizableWheelData | enableAutoTraction | Enable automatic traction control. | bool |
| Wheel | ResizableWheelData | enableSuspension | Enable suspension system. | bool |
| Wheel | ResizableWheelData | engineId | Engine identifier. | int |
| Wheel | ResizableWheelData | hideRims | Hide rims. | bool |
| Wheel | ResizableWheelData | maxAngularVelocity | Maximum angular velocity. | float |
| Wheel | ResizableWheelData | size | Size/scale related setting. | float |
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
| Wheel | ResizableWheelData | width | Size/scale related setting. | float |
| Wheel Suspension | JWheelSuspensionData | damper | Damping factor. | float |
| Wheel Suspension | JWheelSuspensionData | extension | Suspension extension. | float |
| Wheel Suspension | JWheelSuspensionData | rideHeight | Ride height. | float |
| Wheel Suspension | JWheelSuspensionData | shockPosition | Shock position. | float |
| Wheel Suspension | JWheelSuspensionData | size | Size/scale related setting. | float |
| Wheel Suspension | JWheelSuspensionData | stiffness | Stiffness coefficient. | float |
| Wheel Suspension | JWheelSuspensionData | suspensionLength | Suspension travel length. | float |
| Winch | WinchData | attachPoint | Configures attachPoint for Winch. | int |
| Winch | WinchData | breakScale | Break threshold scale. | float |
| Winch | WinchData | range | Operational range/travel. | float |
| Winch | WinchData | speed | Speed/time process setting. | float |
| Winch | WinchData | startRange | Initial cable/range value. | float |
| Winch | WinchData | volume | Volume parameter. | float |
| Wing | JWingData | axis | Axis mapping. | string |
| Wing | JWingData | chordSamples | Chord sampling count. | int |
| Wing | JWingData | colliderSamples | Collider sampling count. | int |
| Wing | JWingData | disableWingtipVortices | Disable wingtip vortices. | bool |
| Wing | JWingData | flipped | Flip airfoil orientation. | bool |
| Wing | JWingData | fuelFraction | Fuel fraction. | float |
| Wing | JWingData | invert | Invert output. | bool |
| Wing | JWingData | invertOnMirror | Invert on mirrored part. | bool |
| Wing | JWingData | liftScale | Lift scaling factor. | float |
| Wing | JWingData | partIds | Referenced part ID list. | string |
| Wing | JWingData | style | Wing style compatibility field used mainly for migration/legacy data. | string (legacy compatible style marker) |
| Wing | JWingData | version | Serialized data version. | int |
| Wing | JWingData | viscousDragScale | Viscous drag scaling factor. | float |
| Wing | JWingData | zeroLiftDragScale | Zero-lift drag scale. | float |
| Wing | WingData | airfoil | Airfoil type. | string |
| Wing | WingData | allowControlSurfaces | Allow control surface usage. | bool |
| Wing | WingData | angleOfAttack | Angle of attack parameter. | float |
| Wing | WingData | baseThickness | Base/root thickness. | float |
| Wing | WingData | density | Density parameter. | float |
| Wing | WingData | fuelPercentage | Fuel percentage. | float |
| Wing | WingData | hingeDistance | Hinge distance. | float |
| Wing | WingData | inverted | Inverted flag. | bool |
| Wing | WingData | liftScale | Lift scaling factor. | float |
| Wing | WingData | minSectionLength | Minimum section length. | float |
| Wing | WingData | rootLeadingOffset | Root leading-edge offset. | float |
| Wing | WingData | rootTrailingOffset | Root trailing-edge offset. | float |
| Wing | WingData | tipLeadingOffset | Tip leading-edge offset. | float |
| Wing | WingData | tipPosition | Tip position. | Vector3(x,y,z) |
| Wing | WingData | tipThickness | Tip thickness. | float |
| Wing | WingData | tipTrailingOffset | Tip trailing-edge offset. | float |
