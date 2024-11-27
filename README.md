Versatile Robot
A Mobile Manipulator with Advanced Capabilities

This repository contains the Versatile Robot, a mobile manipulator capable of navigation, SLAM, and manipulation tasks. This robot is an advanced version of the robot originally developed by Rishikesh Jadhav during his project at the University of Maryland. His foundational work has made this project possible.

Reference: Rishikesh Jadhav's GitHub Repository

Features Added
Sensors:

Integrated a 2D LiDAR for mapping and localization.
Added a Stereo Camera for future vision-based capabilities.
SLAM Capability:

Enabled Simultaneous Localization and Mapping (SLAM) using ROS packages.
Autonomous Navigation:

Configured the Move Base package for autonomous navigation and obstacle avoidance.
Manipulation:

Implemented motion planning and manipulation using the MoveIt! package.
New Simulation Environment:

Added an obstacle-rich environment for the robot to navigate, inspired by the CPR Obstacle World package.
What’s Coming Next
Camera for Manipulation:

Adding a camera to the manipulator for visual manipulation.
Visual Odometry:

Enhancing the robot’s localization with Visual-Odometry capabilities.
Physical Upgrades:

Improving the robot’s physical hardware, such as better wheels and structural enhancements.
Transition to ROS2:

Upgrading the robot’s software stack to ROS2 for better performance and scalability.
More Enhancements:

Additional exciting features are planned—stay tuned!
Installation and Usage
To set up and use the Versatile Robot in your workspace, follow these steps:

Clone the Repository:

bash
Copy code
git clone <your-repo-link>  
cd versatile_robot  
Build the Workspace:

bash
Copy code
catkin_make  
source devel/setup.bash  
Launch the Simulation:

Use the included launch files to test different features:
Manipulation Demo:
bash
Copy code
roslaunch robot_arm arm_Demo.launch  
SLAM and Navigation:
bash
Copy code
roslaunch robot_arm navigate_Robot.launch  
