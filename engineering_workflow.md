# Engineering Workflow

The robotic arm was developed using an iterative engineerng design process. Each stage of development was valdated before progressing to the next, allowing engineering decision to be supported by research, calculations, prototyping and continuous design improvements. 

### 1. Define Mission Requirements
The robotic arm was designed to perform scientific tasks required in the European Rover Challenge (ERC) including drilling, object manipulation and sample retrieval. The primary objective was to develop a lightweight reliable 6 DOF arm capable of operating in a simulated Mars like environment. 

### 2. Background Research
Existing ERC robotic arms and published research on 6-DOF arms were studied to understand a common mechanical arm design and joint configurations. This research provided a foundation for the initial concept. 

### 3. Initial Concept Design
An initial mechanical concept was developed to determine the overall geometry, joint arrangement and approximate dimensions of the robotic arm. The first design targeted a maximum reach of 1.4m to maximise the operational workspace. 

### 4. Motor Selection
A list of candidate motors were created and evaluated by comparing torque output, weight, dimensions, operating voltage and overall suitability for each joints. The most appropriate motors were selected for the waist, shoulder, elbow, wrist joints and the gripper based on the inital design requirements. To see full list click here: [Motor Selection](motor_selection.md)

### 5. Torque Analysis
Static torque analysis was performed for every joint to verify whether the selected motors could safel support the arm under maximum loading conditions, which in this tournament was 1kg. The analysis identified the wrist yaw joint as teh primary limiting factor. To see full analysis click here: [Torque Analysis](torque_analysis.md)

### 6. Design Optimisation 
The torque analysis showed that the initial 1.4m design exceeded the capabilities of the selected wrist actuator. To maintain a lightweight structure without changing the motor configuration, the maximum reach was reduced to 1.0m before continuing the detailed design. 

### 7. Detailed CAD Design
The complete robotic arm ws designed in Autodesk Fusion 360. Custom motor housings, structural members, mounting interfaces and the gripper assembly were developed while ensuring manufacturability and ease of assembly. 

### 8. Prototype Manufacturing
Prototype components were manufactured through 3D printing to verify part dimensions, assembly tolerances and overall mechanical functionality before machining the final aluminium components. 

### 9. Assembly & Validtion
The prototype was assembled and evaluated to identify mechanical issues, dimensional inaccuracies and assembly challenges. Several design revisions were required before the final manufacturing stage. 

### Final Manufacturing (In Progress)
Following multiple design iterations, the robotic arm is currently being manufactured using aluminium structural components for the final competition version. 

