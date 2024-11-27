# Versatile Robot

**A Mobile Manipulator with Advanced Capabilities**

This repository contains the **Versatile Robot**, a mobile manipulator capable of **Navigation**, **SLAM**, and **Manipulation** tasks. This robot is an advanced version of the robot originally developed by **Rishikesh Jadhav** during his project at the University of Maryland. His foundational work has made this project possible
([Rishikesh Jadhav's GitHub Repository](https://github.com/Rishikesh-Jadhav/Mobile-Manipulator-Robot-modeling-and-simulation-using-Gazebo-ROS-Noetic-)).


**DOF (9)** = Robotic arm DoF **(6)** + Mobile robot DoF **(3)**

![imp](https://github.com/user-attachments/assets/3a7a8957-02ba-49c8-95f0-2de73890a46b)


---

## Features Added

1. **Sensors**:
   - Integrated a **2D LiDAR** for mapping and localization.
   - Added a **Stereo Camera** for future vision-based capabilities.

2. **SLAM Capability**:
   - Enabled Simultaneous Localization and Mapping (SLAM) using **[slam_toolbox](https://github.com/SteveMacenski/slam_toolbox)**.

3. **Autonomous Navigation**:
   - Configured the **[move_base](http://wiki.ros.org/move_base)** package for autonomous navigation and obstacle avoidance.

4. **Manipulation**:
   - Implemented motion planning and manipulation using the **[MoveIt!](https://github.com/moveit/moveit)** framework.

5. **New Simulation Environment**:
   - Added an obstacle-rich environment for the robot to navigate, inspired by the **[CPR Obstacle World](https://github.com/clearpathrobotics/cpr_gazebo/tree/noetic-devel/cpr_obstacle_gazebo)** package.

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
## Prerequisites

- This project is developed for **ROS1** (tested on **Noetic**) and is planned to be **upgraded** to ROS2 in future iterations.

1. **Install MoveIt**:
   ```bash
   sudo apt-get update
   sudo apt-get install ros-noetic-moveit

2. **Install SLAM Toolbox**:
   ```bash
   sudo apt-get install ros-noetic-slam-toolbox

3. **Install Move Base**:
   ```bash
   sudo apt-get install ros-noetic-move-base

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

In the **second terminal**, choose **one of the following** based on your task:

- For **SLAM**
   ```bash
   roslaunch robot_arm map_Robot.launch

![n_3](https://github.com/user-attachments/assets/e18bbf94-1f40-4694-be2f-4082ec7a6f64)


- For **Navigation** Only
   ```bash
   roslaunch robot_arm navigate_Robot.launch

![n_1](https://github.com/user-attachments/assets/65c851ca-0b16-468f-ba7e-72c17ddc7ce4)


- For **Navigation** and **Manipulation**
   ```bash
   roslaunch robot_arm navigate_Manipulate_Robot.launch

![n_4](https://github.com/user-attachments/assets/71b8f05b-3612-451c-8431-118f0a850d66)


- **Optional**: To work only with the **MoveIt!** motion planning plugin in RViz
   ```bash
   roslaunch robot_arm arm_Demo.launch

- Also, to adapt the **Motion Planning** settings of the Arm to your needs, you can use **MoveIt Setup Assistant**
   ```bash
   roslaunch moveit_setup_assistant setup_assistant.launch

![n_2](https://github.com/user-attachments/assets/e437355f-ccb2-4325-aa70-3c0d532e12fa)

   
## If you have any question about anything, please feel free to ask! ##
