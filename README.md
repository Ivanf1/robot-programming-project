# Robot Programming Project

This project was developed for the Robot Programming Course.

## Robot

![Robot](https://github.com/Ivanf1/robot-programming-project/raw/main/assets/robot.png)

### Video

[![Robot Video](https://img.youtube.com/vi/MUSglA3YPQ4/0.jpg)](https://www.youtube.com/watch?v=MUSglA3YPQ4)

## Project description

### Idea

Our goal was to build a real robot to better learn ROS and its benefits in a real world application.

Having already many components like motors, Raspberries and Arduinos, we tried to envision what kind of robot we could build.

Our initial idea was to build an hexapod, but unfortunately, some of the motors were broken so we didn't have enough of them to make it work.

After some brainstorming, we decided to build a wheeled robot with an arm capable of grabbing objects.

We also thought it would be interesting to use mecanum wheels to allow different kinds of movements compared to a traditional differential drive robot.

### Components

The robot is built using the following components:

- **Raspberry Pi 4**: Runs Ubuntu 20.04.5 and ROS Noetic, serving as the main processing unit.
- **7 Servo AX-12+**: Used for precise movement and control of the robot's wheels and arm.
- **Arduino Uno with Dynamixel Shield**: Handles communication with the servos motors.
- **Logic Level Converter**: Ensures proper voltage levels between the Raspberry Pi and Arduino.
- **Pi Zero 2 with Pi Camera**: Provides vision capabilities.

### Schematic

The schematic below illustrates the wiring and connections between the robot's components, including the Raspberry Pi, Arduino, servos, and sensors.

![Schematic](https://github.com/Ivanf1/robot-programming-project/raw/main/assets/schematic.jpg)

### Mecanum wheels motion

Mecanum wheels enable the robot to move in any direction without needing to rotate. This unique capability is achieved by the angled rollers on each wheel, which allow for omnidirectional movement. The diagram below demonstrates the motion patterns possible with mecanum wheels and the equation used to control the motion.

![Mecanum](https://github.com/Ivanf1/robot-programming-project/raw/main/assets/mecanum.svg)

### Ros nodes graph

The ROS nodes graph provides a visual representation of the communication between different components of the robot.

![RosNodeGraph](https://github.com/Ivanf1/robot-programming-project/raw/main/assets/rosgraph.svg)

## Linked repositories

| Repository Name                                                            | Description                                                                   |
| -------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| [robot-motor-controller](https://github.com/Ivanf1/robot-motor-controller) | Code for managing motor control, including speed, direction, and movement.    |
| [robot-ros](https://github.com/Ivanf1/robot-ros)                           | ROS packages for communication, navigation, and sensor integration.           |
| [robot-controller-app](https://github.com/Ivanf1/robot-controller-app)     | A mobile application for remotely controlling the robot.                      |
| [robot-3d-model](https://github.com/Ivanf1/robot-3d-model)                 | 3D models and simulation files for testing the robot in virtual environments. |
