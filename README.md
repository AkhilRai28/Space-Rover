# GUJCOST Project - Autonomous Planetary Rover

## Project Overview

This project involves the development of an autonomous planetary rover using the ROS framework on Ubuntu 20.04. The rover is designed to navigate rugged terrain autonomously, equipped with various sensors and a custom suspension system to ensure stability and effectiveness in harsh environments.

## Outcomes

1. Implemented advanced navigation algorithms to enhance obstacle avoidance by 40%.
2. Developed a web-based GUI for real-time control and monitoring of the rover.
3. Designed and 3D-printed custom suspension and wheel components, improving terrain handling and durability.
4. Integrated sensors and electronic components to achieve robust autonomous functionality.

## Table of Contents

1. [Dual Booting](#dual-booting)
2. [ROS Installation and Terminologies](#ros-installation-and-terminologies)
3. [ROS Commands](#ros-commands)
4. [Publisher-Subscriber Files](#publisher-subscriber-files)
5. [Rover Simulation](#rover-simulation)
6. [Hardware Integration](#hardware-integration)
7. [Web GUI](#web-gui)
8. [Navigation Algorithms](#navigation-algorithms)
9. [Suspension System](#suspension-system)
10. [Errors Encountered](#errors-encountered)
11. [Bibliography](#bibliography)

## Dual Booting

- **Setup**: Installed Ubuntu 20.04 alongside an existing operating system (typically Windows) to enable a dual-boot configuration.
- **Tools Used**: Used Rufus 4.1 for creating a bootable USB drive with the Ubuntu installation ISO.
- **Purpose**: This setup was necessary to run ROS (Robot Operating System) which is best supported on Ubuntu.

## ROS Installation and Terminologies

- **Installation**: Followed official ROS Noetic installation guidelines for Ubuntu 20.04, setting up the environment with essential packages and dependencies.
- **Key Concepts**:
  - **Nodes**: Independent processes that perform computation.
  - **Topics**: Channels over which nodes exchange messages.
  - **Packages**: Collections of nodes, data, and configuration files.
  - **Workspaces**: Directories where ROS packages are stored and managed.

## ROS Commands

- **Basic Commands**:
  - `roscore`: Starts the ROS master, which coordinates communication between nodes.
  - `rosnode`: Manages nodes; commands include `rosnode list` and `rosnode info`.
  - `rosrun`: Runs a node from a specified package.
  - `rostopic`: Manages topics; commands include `rostopic list` and `rostopic echo`.
  - `roslaunch`: Launches multiple nodes and configurations from a single file.

## Publisher-Subscriber Files

- **Publisher**: A ROS node that sends data to a topic.
- **Subscriber**: A ROS node that receives data from a topic.
- **Implementation**: Created ROS nodes that publish and subscribe to topics to facilitate communication between different parts of the system, such as sensor data from hardware to a control algorithm.

## Rover Simulation

- **Gazebo**: Used Gazebo to simulate the rover in various terrains, testing the navigation and obstacle avoidance algorithms.
- **RVIZ**: Utilized RVIZ for visualization and debugging, enabling real-time adjustments to the rover's navigation system.

## Hardware Integration

- **Components**:
  - **Ultrasonic Sensors (HCSR04)**: Used for distance measurement and obstacle detection.
  - **Lidar**: For 3D mapping and advanced navigation.
  - **Cameras**: Provide visual data for obstacle recognition.
  - **Motor Drivers**: Control the speed and direction of motors.
  - **Arduino**: Microcontroller for processing sensor data and controlling motors.
- **Assembly**: Detailed steps for assembling the rover hardware and connecting the components to the Arduino.

## Web GUI

- **Functionality**: Developed a web-based GUI for real-time control and monitoring, allowing users to input navigation commands and visualize sensor data remotely.
- **Technologies Used**: Implemented using HTML, CSS, JavaScript, and Flask for the backend server.

## Navigation Algorithms

- **Goal-To-Goal Navigation**: Developed algorithms to navigate the rover from one goal point to another.
- **PID Controller**: Implemented a Proportional-Integral-Derivative (PID) controller to maintain the desired trajectory and speed while avoiding obstacles.
- **Vector-Based Algorithm**: Enhanced obstacle avoidance by calculating resultant vectors from multiple sensors to direct the rover away from obstacles and towards the goal.

## Suspension System

- **Design**: Utilized a double lambda rocker-bogie suspension system to maintain stability on uneven terrain.
- **3D Printing**: Designed and printed custom wheels and suspension components to ensure durability and performance.

## Errors Encountered

- **Documentation**: Recorded various issues faced during development, including software bugs, hardware malfunctions, and integration challenges.
- **Solutions**: Provided troubleshooting steps and solutions for each error encountered.

## Bibliography

- [ROS Official Website](https://www.ros.org/)
- [What is ROS? - Ubuntu Robotics](https://ubuntu.com/robotics/what-is-ros)
- [Dual Boot Guide - FreeCodeCamp](https://www.freecodecamp.org/news/how-to-dual-boot-any-linux-distribution-with-windows/)
- [ROS Commands Summary - Packt](https://subscription.packtpub.com/book/iot-and-hardware/9781788479592/1/ch01lvl1sec15/ros-commands-summary)

---

Feel free to customize the sections based on your specific project details and requirements.
