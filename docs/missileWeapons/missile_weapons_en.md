# Missile Weapon Lock-on Duration

## 1. Lock-on Time Calculation

### 1.1 Lock-on Rate $r$

- First, compute the lock-on rate $r$:
  $$
  r=\max\left(\mathrm{clamp}\left(\frac{\text{signature}}{\text{distance}}\cdot \text{SeekerSensitivity},\,0,\,2\right),\,0.1\right)
  $$
- If it is a continuous-illumination lock, multiply by $1.5$:
  $$
  r \leftarrow 1.5r
  $$

### 1.2 Lock Progress $L$

- Lock progress updates as:
  $$
  L_{t+\Delta t}=\min(1,\,L_t+r\Delta t)
  $$
  where $L$ is the lock progress percentage. When $L=1$, the target is considered fully locked.
- After canceling lock on the target, lock progress decays as:
  $$
  L_{t+\Delta t}=\max(0,\,L_t-0.5\Delta t)
  $$

### 1.3 Theoretical Lock Time (without interference)

$$
T_{\text{lock}}=\frac{1}{r}
$$

## 2. Key Parameters

### 2.1 SeekerSensitivity

- Infrared seeker: 5
- Radar seeker: 25
- Laser seeker: 2500
- Anti-radiation seeker: 5

### 2.2 Signature (target signal strength)

> This parameter represents the target signal strength received by the missile seeker, and is affected by both target type and seeker type.

#### 2.2.1 Signature values against ground targets

- Infrared seeker: 100
- Radar seeker: 50
- Anti-radiation seeker: 250

#### 2.2.2 Signature values against laser-designator targets

- Laser seeker: 1

#### 2.2.3 Signature values against player targets

##### Generic seekers

- Unguided: 0
- Laser seeker: 0
- Anti-radiation seeker: 100

##### Infrared / Radar seekers (player aircraft)

The calculation is more complex and changes dynamically with the player aircraft state.

###### Infrared seeker

1. First compute target infrared value `targetIR`:
   - If fuel is available: iterate all engines currently connected to the cockpit and sum each engine's infrared Signature;
   - then multiply by `0.25`;
   - if no fuel: `targetIR = 0`.
2. Then apply smoothing:
   - `IRSignature = StepTowards(IRSignature, 250f * deltaTime, targetIR)`

That is:

$$
IR_{target}=
\begin{cases}
0.25\cdot\sum IR_{engine}, & Fuel>0 \\
0, & Fuel\le 0
\end{cases}
$$

$$
IR_{new}=StepTowards(IR_{old},\,250\cdot\Delta t,\,IR_{target})
$$

IRSignature calculation differs by engine type:

- Jet engine (normal state) IRSignature = current throttle * power multiplier * max power * 1
- Jet engine (afterburner state) IRSignature = jet normal-state IRSignature * Lerp(1, 10, afterburnerPercent)
- Rotor/propeller IRSignature = jet normal-state IRSignature * 0.1
- Vehicle engine IRSignature = current throttle * max power * 0.5

Afterburner throttle percentage:

$$
afterburnerPercent=\mathrm{clamp01}\left(\frac{\text{throttle}-\text{AfterburnerThrottleStart}}{1-\text{AfterburnerThrottleStart}}\right)
$$

###### Radar seeker

Algorithm:

1. Sum each part's drag values in six directions (up, down, left, right, front, back);
2. then add current wing surface area.

So:

$$
RadarSignature=\sum_{part}(D_f+D_b+D_l+D_r+D_d+D_u)+WingSurfaceArea
$$

Notes:

1. The “drag” here is not traditional aerodynamic drag; it is closer to an effective drag-area engineering quantity, so the unit is not Newton.
2. Part XML attributes `dragScale` and `calculateDrag` also affect radar signature calculation.
3. Since radar signature also includes wing area, setting all part drag values to 0 still leaves a radar signature; and even with no wings, lock-on still has a minimum rate of `0.1` per second, so **true radar invisibility is not achievable**.

---

## 3. Extra Mechanisms That Slow or Reset Lock

- When the target's `evade/break lock probability` increases, a random check is triggered;
- if that check fails, then:
  - `LockPercentage = 0`
  - `_timeUntilCanLock = 1.5f` (a 1.5-second cooldown before lock can start again)

These probabilities mainly come from the `PlayerTarget` + countermeasure script chain:

- `PlayerTarget.cs` (`AddEvadeLockProbability` / `AddBreakLockProbability`)
- `CounterMeasureScript.cs`
- `CounterMeasureDispenserData.cs`

---

## 4. Key Non-XML (Hardcoded / Code-Constant) Items

- Lock rate clamp range: `0 ~ 2` (with a minimum floor of `0.1` afterward)
- Continuous-lock multiplier: `1.5`
- Decay when not locking: `0.5/s`
- Cooldown after interference: `1.5s`
