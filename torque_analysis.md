# Torque Analysis 
## Objective
One of the most critical stages of the designing process was verifying whether or not the selected motors could support the robotic arm throughout its operating range. 

Therefore, rather than selecting motors based entirely on manufacturer specifications, a complete static torque analysis was performed to determine the torque demand at each joint under maximum loading conditions. 

This analysis was used to validate the mechanical design, identify potential failure points and guide subsequent design decisions before manufacturing. <br>
The primary objectives of the analysis were to:
- Verify that each motor could safely support the expected loads.
- Determine the maximum feasible arm reach using the selected motors.
- Idenfity the limiting joint within the mechanical system.
- Idenfity the maximum weight the arm could withstand relative to specific arm reach.
- Optimise the design while maintaining a lightweight structure.

## Initial Design Assumptions
The inital robotic arm was designd with the following target specifications:
| Parameter | Value |
|-----------|------:|
| Initial Reach | 1.4 m |
| Structural Mass (excluding payload) | 2.0 kg |
| Payload | 1.0 kg |
| Gravitational Acceleration | 9.8 m/s² |

The initial design prioritised maximum operational workspace. However, there assumptions required engineering validation before detailed manufacturing could begin. 

## Engineering Methodology

A static torque analysis was carried out for every joint using classical rigid-body mechanics. 

For every joint, the following procedure was applied: 
1. Determine the remaining structural mass supported by the joint.
2. Calculate the effective lever arm to the centre of mass of each component.
3. Compute the gravitational force acting on each component.
4. Calculate the individual torque contributions.
5. Sum all torque contributions to determine the total required holding torque.
6. Compare the calculated torque demand with the peak torque specifictionn of the selected motor.

This sequential approach allowed each joint to be evaluated independently while accurately representing the physical loading conditions experienced during operation.

## Governing Equation
The required holding torque of each joint was calculated using the fundamental moment equation. 
`τ = Σ(F × d)`

Since force is defined as:

`F = m × g`

the governing equation becomes:

`τ = Σ(m × g × d)`

where:

- **τ** = Required holding torque (Nm)
- **m** = Mass of each component (kg)
- **g** = Gravitational acceleration (9.81 m/s²)
- **d** = Perpendicular distance from the joint axis to the component's centre of mass (m)


---

## Step 1 - Downstream Mass Analysis
Rather than analysing the robotic arm as a single structure, each joint was evaluated independently by considering the components located downstream of its axis of rotation. 

As the analysis progresses from the shoulder towards the end effector, both the supported mass and the effective lever arm decrease. 

For example: 
### Shoulder Joint
Supports:
- Link 1 (Aluminium 3030)
- Link 2 (Aluminium 2020)
- Wrist Assembly
- Gripper
- Payload

### Elbow Joint
Supports:
- Forearm
- Wrist Assembly
- Gripper
- Payload

### Wrist Joint
Supports:
- Wrist Assembly
- Gripper
- Payload

This methodology allowed each joint to be analysed independently while accurately modelling the physical behaviour of the robotic arm. 

## Step 2 - Shoulder Joint Analysis
The shoulder motor has to support the entire robotic arm together with the payload added as well. 

### Components
| Component | Mass (kg) | Distance (m) |
|-----------|----------:|-------------:|
| Link 1 | 0.5329 | 0.225 |
| Remaining Structure | 1.4671 | 0.925 |
| Payload | 1.000 | 1.400 |

The total required torque is<br>
`τ = (0.5329 x 9.81 x 0.225) + (1.4671 x 9.81 x 0.925) + (1.0 x 9.81 x 1.4)`<br>
`τ  = 1.176 + 13.313 + 13.734`<br>
**Required Torque = 28.223 Nm**
| Motor Specification | Value |
|---------------------|------:|
| Maximum Torque | 30.0 Nm |
| Required Torque | 28.223 Nm|
| Safety Margin | 1.777 Nm |

**Result: ** Pass<br>
The shoulder motor operates within its maximum torque capability and provides an acceptable safety margin. 

---

## Joint 3 - Elbow Pitch
The elbow supports only the downstream portion of the robotic arm. <br>
The following componets were removed from the calculations:
- Link 1
- Shoulder assembly
- Shoulder Motor mass
### Remaining Parameters
 Parameter | Value |
|-----------|------:|
| Remaining Mass | 1.205724 kg |
| Remaining Reach | 0.95 m |
| Centre of Mass | 0.475 m |
| Payload Distance | 0.95 m |

The required holding torque becomes<br>

`τ = (1.205724 × 9.81 × 0.475) + (1.0 × 9.81 × 0.95)`<br>

`τ = 5.618 + 9.319`<br>

**Required Torque = 14.937 Nm**

| Motor Specification | Value |
|---------------------|------:|
| Rated Torque | 30.0 Nm |
| Required Torque | 14.937 Nm |

**Result: ** Pass

## Joint 4 – Wrist Yaw

The wrist yaw actuator proved to be the limiting joint of the robotic arm.

After removing all upstream components, only the wrist assembly and payload remained.

### Remaining Parameters

| Parameter | Value |
|-----------|------:|
| Remaining Mass | 0.957323 kg |
| Effective Reach | 0.329 m |
| Centre of Mass | 0.1645 m |

The required holding torque becomes<br>

`τ = (0.05 × 9.81 × 0.1645) + (1.0 × 9.81 × 0.329)`<br>
`τ = 0.081 + 3.227`<br>
**Required Torque = 3.308 Nm**

| Motor Specification | Value |
|---------------------|------:|
| Peak Torque | 3.0 Nm |
| Required Torque | 3.308 Nm |

**Result: ** Fail<br>
The calculated torque exceeds the peak torque capability of the selected motor, making the original 1.4m design mechanically infeasible. 

## Joint 5 – Wrist Pitch

### Remaining Parameters

---

| Parameter | Value |
|-----------|------:|
| Remaining Reach | 0.306 m |

The required holding torque becomes<br>

`τ = (0.00625 × 9.81 × 0.0115) + (1.0 × 9.81 × 0.306)`<br>

`τ = 0.0007 + 3.002`<br>

**Required Torque = 3.003 Nm**

| Motor Specification | Value |
|---------------------|------:|
| Peak Torque | 3.0 Nm |
| Required Torque | 3.003 Nm |

**Result:** Stall Limit

The motor operates almost exaclty at its maximum capability and would have little or no available torque for dynamic motion. 

---
## Joint 6 – Gripper Roll

### Remaining Parameters

| Parameter | Value |
|-----------|------:|
| Remaining Reach | 0.1975 m |

The required holding torque becomes<br>

`τ = (0.066235 × 9.81 × 0.0542) + (1.0 × 9.81 × 0.1975)`<br>

`τ = 0.035 + 1.937`<br>

**Required Torque = 1.972 Nm**

| Motor Specification | Value |
|---------------------|------:|
| Rated Torque | 2.0 Nm |
| Required Torque | 1.972 Nm |

**Result:** Pass

The motor is capable of holding the payload statically but operates at approximately 98.6% of its continuous torque limit. 

## Summary of Results
| Joint | Reach (m) | Required Torque (Nm) | Motor Capacity (Nm) | Status |
|------|----------:|---------------------:|--------------------:|:------:|
| Shoulder (J2) | 1.400 | 28.223 | 30.0 | PASS |
| Elbow (J3) | 0.950 | 14.937 | 2.0 | PASS |
| Wrist Yaw (J4) | 0.329 | 3.308 | 3.0 | FAIL |
| Wrist Pitch (J5) | 0.306 | 3.003 | 3.0 | STALL |
| Gripper Roll (J6) | 0.197 | 1.972 | 2.0 | PASS |

## Engineering Optimisation

The wrist yaw joint was identified as the primary mechanical bottleneck.

Rather than replacing the actuator with a larger and heavier motor, the governing torque equation was rearranged to determine the allowable payload and maximum reach while retaining the existing actuator.

### Maximum Allowable Payload

`Maximum Payload = Motor Torque / (Gravity × Distance)`<br>

`= 3.0 / (9.81 × 0.329)`

**Maximum Payload = 0.93 kg**

### Critical Reach

`Maximum Reach = Motor Torque / (Payload × Gravity)`

`= 3.0 / (1.0 × 9.81)`

**Critical Reach = 0.306 m**

To achieve a dynamic safety factor of approximately **1.3×**, the wrist assembly should be shortened from **329 mm** to approximately **235 mm**.

This analysis directly influenced the final mechanical design and led to the decision to reduce the overall arm reach from **1.4 m** to **1.0 m**, ensuring that the robotic arm remained lightweight while operating within the capabilities of the selected actuators.


