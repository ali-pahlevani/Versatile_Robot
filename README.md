# Versatile Robot

**A Mobile Manipulator with Advanced Capabilities**

This repository contains the **Versatile Robot**, a mobile manipulator capable of navigation, SLAM, and manipulation tasks. This robot is an advanced version of the robot originally developed by **Rishikesh Jadhav** during his project at the University of Maryland. His foundational work has made this project possible.

**Reference**: [Rishikesh Jadhav's GitHub Repository](https://github.com/Rishikesh-Jadhav/Mobile-Manipulator-Robot-modeling-and-simulation-using-Gazebo-ROS-Noetic-)

---

## Features Added

1. **Sensors**:
   - Integrated a **2D LiDAR** for mapping and localization.
   - Added a **Stereo Camera** for future vision-based capabilities.

2. **SLAM Capability**:
   - Enabled **Simultaneous Localization and Mapping (SLAM)** using ROS packages.

3. **Autonomous Navigation**:
   - Configured the **Move Base** package for autonomous navigation and obstacle avoidance.

4. **Manipulation**:
   - Implemented motion planning and manipulation using the **MoveIt!** package.

5. **New Simulation Environment**:
   - Added an obstacle-rich environment for the robot to navigate, inspired by the **CPR Obstacle World** package (https://github.com/clearpathrobotics/cpr_gazebo/tree/noetic-devel/cpr_obstacle_gazebo).

---

## What’s Coming Next

1. **Camera for Manipulation**:
   - Adding a camera to the manipulator for **visual manipulation**.

2. **Visual Odometry**:
   - Enhancing the robot’s localization with **Visual-Odometry** capabilities.

3. **Physical Upgrades**:
   - Improving the robot’s physical hardware, such as **better wheels** and structural enhancements.

4. **Transition to ROS2**:
   - Upgrading the robot’s software stack to **ROS2** for better performance and scalability.

5. **More Enhancements**:
   - Additional exciting features are planned—stay tuned!

---

## Installation and Usage

**To set up and use the Versatile Robot in your workspace, follow these steps:**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ali-pahlevani/Versatile_Robot.git
   cd Versatile_Robot

2. **Build the Workspace**:
   ```bash
   catkin_make
   source devel/setup.bash

3. **Launch the Simulation**:
In one terminal, launch the main simulation:
   ```bash
   roslaunch robot_arm main_Launch.launch
This loads the world in Gazebo, spawns the robot, and initializes the controllers.

In the second terminal, choose **one of the following** based on your task:

- For **SLAM**
   ```bash
   roslaunch robot_arm main_Launch.launch

- For **Navigation** Only
   ```bash
   roslaunch robot_arm navigate_Robot.launch

- For For **Navigation** and **Manipulation**
   ```bash
   roslaunch robot_arm navigate_Manipulate_Robot.launch

- **Optional**: To work only with the **MoveIt!** motion planning plugin in RViz
   ```bash
   roslaunch robot_arm arm_Demo.launch
   
![2](https://github.com/user-attachments/assets/0121c105-42c1-49b2-9926-8f1278f8498f)


