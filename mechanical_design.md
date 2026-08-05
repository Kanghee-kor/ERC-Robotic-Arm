## Mechanical Design
The robotic arm was designed entirely in Autodesk Fusion 360 using a modular design philosohpy. Each joint and structural component was developed as an indepented assembly, allowing individual parts to be modified without redesigning the entire system. Throughout the process, the design balanced four competing priorities: Structural rigidity, low weight, manufacturibility and ease of assembly. 

---

## Overall Architecture
The arm consists of six rotational joints, providing the six degrees of freedom needed for the manipulation tasks required in the challenge. 

The mechanical structure is built from aluminium 2020 & 3030 extrusion, custom designed motor housings, structural connection brackets and a custom designed gripper:

- Waist Joint: The bottom most joint responsible for the free 360 degrees turning of the arm.
  Needs enough torque to turn the entire arm weight and the payload.
  
- Shoulder and Elbow Joints: These joints provide the primary lifting capabiltiy, supporting te majority of the arm's mass and the payload.

- Wrist joints: This joint controls the orientation of the end effector for scienctific operation.

- Gripper: A custom designed end effector for object manipulation

The modular architecture means individual joints and components can be redesigned or replaced without affecting the rest of the system. This was a deliberate choice that paid off during the manufacturing stage, when several housings needed rework. Check here for more information: [Manufacturing & Assembly](manufacturing.md)

`Place photo of complete CAD model of the arm`

---

## CAD Development
Development began wit te overall mechanical layout, then moved into the detailed design of eac joint and structural memeber. 

Imported Components: 
- CAD models provided directly by motor manufactureres were imported into the assemly to ensure accurate dimension, mounting interfaces and mechanical clearances.

- Standard 2020 & 3030 aluminium extrusion profiles were imported.

Custom Designed Components:
- Motor Housings

- Connection Brackets

- Structural Interaces

- Gripper

Check [Motor Selection & Torque Analysis](torque_analysis.md)for how each motors were chosen. 

Simulation and Verification. Fusion 360 joint simulations were used throughout development to:
1. Verify range of motion at each joint

2. Evaluate joint movement under the full assembly

3. Identify potential mechanical interference before committing to manufacturing

This simulate before building caught several clearance issues early, reducing the number of aluminium prototype iterations needed later. 

---
