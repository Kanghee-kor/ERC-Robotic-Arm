# ERC-Robotic-Arm
Design and development of a 6-DOF robotic arm for the European Rover Challenge (ERC).
---

# Project Overview
The ERC Robot Arm is a multidisciplinary engineering project developed for the European Rover Challenge, an international robotic competition that simulates real-world Mars exploration missions.<br> The objective of this project is to design, manufacture and integrate a 6-degree of freedom robotic arm capable of performing a range of scientific tasks such as sample retrieval, object manipulation and drilling operations.<br>
The project follows a complete engineering design process, beginning with mission requirements, progessing through concept development, component selection, mechanical design, engineering analysis, prototype manufacturing and feedback & design improvements.<br>
As the Robot Arm Team Lead, I was responsible for leading the mechanical development of the arm, including motor selection, torque analysis, CAD design, manufacturing planning, technical documentation and project coordination.<br>
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
