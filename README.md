# ERC-Robotic-Arm
Design and development of a 6-DOF robotic arm for the European Rover Challenge (ERC).
---

# Project Overview
The ERC Robot Arm is a multidisciplinary engineering project developed for the European Rover Challenge, an international robotic competition that simulates real-world Mars exploration missions.<br> The objective of this project is to design, manufacture and integrate a 6-degree of freedom robotic arm capable of performing a range of scientific tasks such as sample retrieval, object manipulation and drilling operations.

The project follows a complete engineering design process, beginning with mission requirements, progessing through concept development, component selection, mechanical design, engineering analysis, prototype manufacturing and feedback & design improvements.

As the Robot Arm Team Lead, I was responsible for leading the mechanical development of the arm, including motor selection, torque analysis, CAD design, manufacturing planning, technical documentation and project coordination.

The current phase of the project focuses on completing the mechanical system using aluminium structural components before integrating embedded software. 

# Competition Background
The European Rover Challenge (ERC) is an international robotics competiton that simulates realistic Mars exploration missions. Teams from universities around the world design and build autonomous or semi-autonomous rovers capable of completing scientific tasks in a Mars-like environment. <br>
The robotic arm plays a critical role in these missions by enabling the rover to interact with its surrondings. Typical competition tasks include: 
- Scientific sample retrieval
- Object manipulation
- Drilling operations
- Equipment handling
- Precision interaction with mission hardware<br>

The arm must achieve these objectives while oprating under strict engineering constraints such as limited weight, structural rigidity, payload capacity and reliability. 

# Design Objectives
The primary objective of this project was to design a reliable and lightweight 6-DOF robotic arm capable of completing the scientific tasks required for the ERC competition. 
The design was developed with the following engineering objectives:
- Develop a 6-DOF manipulator capable of performing drilling, sample retrieval and object manipulation tasks.
- Achieve a maximum reach of approximately **1.0 m** while maintaining structural stability.
- Minimise overall weight through the use of aluminium extrusion and 3D-printed components.
- Select motor actuators capable of providing sufficient torque for each joint based on engineering analysis.
- Design nodular structure that allows individual components to be modified or replacedc during future development.
- Validate design decisions through iterative prototyping, manufacturing and mechanical testing.
- Establish a mechanical platform that can support future embedded control and autonomous software integration.

# My Responsibilities
As the **Robot Arm Team Lead**, I was responsible for coordinating the mechanical development of the arm while contributing directly to its engineering design, analysis and manufacturing. My responsibilities included both technical and project management tasks. 

### Mechanical Design
- Designed the complete 6-DOF robotic arm in **Fusion 360**, including the overall mechanical structure, motor integration, custom motor housings and end-effector assembly.
- Developed the mechanical architecture with consideration for structural rigidity, modularity and manufacturability and future system integration.

### Engineering Analysis
- Performed static torque analysis for every joint to determine motor requirements.
- Calculated the maximum allowable raech and payload by analysing the gravitational loading throughout the motor
- Identified the wrist yaw joint as the primary mechanical bottleneck and used the analysis to guide design improvements.

### Motor Selection
- Led the motor selection process by evaluating candidate motors against project requirements.
- Compared motor specifications including peak torque, weight and physical dimensions before selecting the final configuration for each joint.

### Documentation
- Wrote a technical documentation describing the engineering methodology, torque calculations, project risks, design limitations and opportunities for future development.

### Project Coordination
- Planned the development schedule for the robot arm subsystem. 
- Commuicated component requirements to the ERC project lead to support purchasing and procurement. 

# System Specifications
| Category | Specification |
| -----------| -------------|
| Project | ERC 6-DOF Robotic Arm |
| Competition | European Rover Challenge (ERC) |
| Degrees of Freedom | 6 DOF |
| Maximum Reach | 1.0 m |
| Primary Structure | 3030 & 2020 Aluminium Extrusions |
| Prototype Material | PLA (3D Printed) |
| End Effector | Custom Designed Gripper |
| CAD Software | Fusion 360 |
| Current Status | Mechanical Design & Manufacturing |

### Motor Configuration
| Joint | Motor |
|--------|-------|
| Waist | GIM8108-8 |
| Shoulder | GIM4310-40 |
| Elbow | GIM4310-40 |
| Wrist Yaw | STS3215-12V |
| Wrist Pitch | STS3215-12V |
| Wrist Roll | STS3215-12V |
| Gripper | STS3215-12V |

# Engineering Workflow
The robotic arm was developed using an iterative engineering design process. Each stage of development was validated before progressing to the next, allowing engineering decisions to be supported by research, calculations, prototyping and continuous design improvements.
### 1. Define Mission Requirements
The robotic arm was designed to perform scientific tasks required in the European Rover Challenge (ERC), including drilling, object manipulation and samle retrieval. The primary objective was to develop a lightweight, reliable and modular 6 DOF arm capable of operating in a simulated Mars like environment. 
### 2. Background Research
Existing ERC robotic arms and published research on 6-DOF arms were studied to understand common mechanical designs, joint configurations and design examples. This research provided a foundation for the initial concept. 
### 3. Initial Concept Design
An initial mechanical concept was developed to determine the overall geometry, joint arrangement and apporximate dimensions of the robotic arm. THe first design targeted a maximum reach of 1.4 m to maximize the operational workspace. 
### 4. Motor Selection
A list of candidate motors was created and evaluated by comparing torque output, weight, dimensions, operating voltage and overall suitability for each joints. The most appropriate motors were selected for the waist, shoulder, elbow, writst joints and gripper based on the initial design requirements. 
### 5. Torque Analysis 
Static torque analysis was performed for every joint to verify whether the selected motors could safely support the arm under maximum loading conditions, which in this tournament was 1kg. The analysis identified the wrist yaw joint as the primary limiting factor. 
### 6. Design Optimisation
The torque analysis showed that the initial 1.4 m design exceeded the capabilities of the selected wrist actuator. To maintain a lightweight structure without changing the motor configuration, the maximum reach was reduced to 1.0 m before continuing the detailed design. 
### 7. Detailed CAD Design
The complete robotic arm was designed in Autodesk Fusion 360. Custom motor housings, structural members, mounting interfaces and the gripper assembly were developed while ensuring manufacturability and ease of assembly. 
### 8. Prototype Manufacturing
Prototype components were manufactured using PLA through 3D printing to verify part dimensions, assembly tolerances and overall mechanical functionality before machining the final aluminium components. 
### 9. Assembly & Validation
The prototype was assembled and evaluated to identify mechanical issues, dimensional inaccuracies and assembly challenges. Several design revisions were required before the final manufacturing stage. 
### 10. Final Manufacturing (In Progress)
Following multiple design iterations, the robotic arm is currently being manufactured using aluminium structural components for the final competition version. 
# Mechanical Design

The robotic arm was designed entirely in Autodesk Fusion 360 using a modular design philosophy. Each joint and structural component was developed as an independent assembly, allowing individual parts to be modified without redesigning the entire system. The design focused on balancing structural rigidity, low weight, manufacturability, and ease of assembly.

## Overall Architecture

The robotic arm consists of six rotational joints, providing six degrees of freedom for manipulation tasks required in the European Rover Challenge.<br>

The mechanical structure consists of aluminium extrusions, custom-designed motor housings, structural connection brackets, and a custom-designed gripper. The shoulder and elbow joints provide the primary lifting capability, while the wrist joints control the orientation of the end effector for scientific operations.<br>

The modular architecture allows individual joints and components to be redesigned or replaced without affecting the remainder of the system, improving maintainability and future development.

> **Figure 1.** Complete CAD model of the 6-DOF robotic arm.<br>

## Cad Development
The development began with the overall mechanical layout, followed by the detailed design of each joinnt and the overall structure. CAD designs provided by the motor manufacturers were imported directly into the assembly to ensure accurate dimensions, mounting interfaces and mechanical clearances. Standard 2020 & 3030 aluminoum extrusion profiles were also imported to represent the final structural frame accurately.

All remaining mechanical components, such as the motor housings, connection brackets, structural interfaces and the gripper were designed from scratch to integrate the selected motors into the arm so that they could achieve our initial goals of the arm.

Fusion 360 joint simulations were used throughout development to verify the range of motion, evaluate joint movement and identify potential mechanical interference before manufacturing. 

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

---

# Manufacturing & Assembly
## Prototype Manufacturing
Following the completion of the CAD model and torque analysis, a physical prototype was manufactured to validate the mechanical design. 

The structural frame was made using standard 2020 and 3030 aluminium extrusions. Custom motor housings, mounting brackets and gripper componenets were initially manufactured using PLA through 3D printing. 

The use of additive manufacturing allowed rapid iteration and enabled design verification before comitting to machining aluminium components. 

---

## Assembly Process

The robotic arm was assembled progressively, beginning with the primary structural frame before integrating each motor. 

The assembly process included:
- Mounting the aluminium frame
- Fitting custom motor housings
- Installing all motors
- Aligning each rotational joint
- Verifying mehcanical clearances
- Checking joint motion after each assembly stage

Frequent test assemblies were performed throughout the process to ensure all components fit correctly before final manufacturing. 

---

## Manufacturing Challenges

During the manufacturing stage, several issues appeared that were not immediately apparent during CAD development. <br>
Some motor housings required redesign after discovering missing mounting holes and incorrect dimensional tolerances during assembly. <br>
Rather than forcing holes so that the components could fit, the affected parts were redesigned, reprinted and tested aganin until the desired fit and functionality were achieved. <br>
From those processes, the final mechanical design was significantly more detailed and accurate.

---

## Future Manufacturing

Once the PLA prototype has been fully validated, the custom components will be made from aluminium. 

The transition to aluminium is expected to provide:
- Increased structural rigidity
- Improved durability
- Higher load capacity
- Better dimensional accuracy for competition use

The aluminium version is currently planned as the final competition used assembly. 

---

## Engineering Lessons

One of the most valuable lessons from this project has been understanding that a successful CAD model does not always translate directly into a manufacturable product.

Althougt the overall mechanical design was successful, the actual physical assembly exposed several problems which involved tolerance ussues, fastener access and assembly problmes. To solve these problems, multiple redesigning was necessary and it was a reminder that engineering is never completed in one try, but there is always room for feedback. 

This experience strengthened my understanding of rapid prototyping, design for manufacturing and the relationship between digital design and physical implementation. 

# Challenges & Solutions 

