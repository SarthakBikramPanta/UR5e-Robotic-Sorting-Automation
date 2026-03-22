## Project Overview
This project demonstrates a methodical approach to robotic motion control using a Universal Robot UR5e and an RG Gripper . The system uses conditional logic to sort objects based on their physical dimensions (width).

## Key Features
Sensor-Driven Decision Making: Uses get_rg_Width()to dynamically branch the robot's path.

Optimized Motion: Implements Movej(Joint motion) for fast, efficient movement between defined waypoints.

Cyclic Workflow: Features a central hub (Waypoint 3) to ensure repeatable and error-reduced performance.

## Logic Flow
Python
# Simplified Logic Representation
Move to Waypoint_3 (Hub)
Grip Object
If Width >= 25:
    Move to Waypoint_5 (Large Object Zone)
Else:
    Move to Waypoint_6 (Small Object Zone)
Return to Waypoint_3
## Hardware Used
Robot: Universal Robots UR5e (e-Series) 

Tooling: RG Collaborative Gripper 

Reach/Payload: 850 mm / 5 kg 
