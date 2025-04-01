# Robot Programming Project

This project was developed for the Robot Programming Course.

## Robot

![Robot](https://github.com/Ivanf1/robot-programming-project/raw/main/assets/robot.png)

## Project description

### Idea

Our goal was to build a real robot to better learn ROS and its benefits in a real world application.

Having already many components like motors, Raspberries and Arduinos, we tried to envision what kind of robot we could build.

Our initial idea was to build an hexapod, but unfortunately, some of the motors were broken so we didn't have enough of them to make it work.

After some brainstorming, we decided to build a wheeled robot with an arm capable of grabbing objects.

We also thought it would be interesting to use mecanum wheels to allow different kinds of movements compared to a traditional differential drive robot.

### Components

- Raspberry Pi 4 with Ubuntu 20.04.5 and ROS Noetic.
- 7 Servo AX-12+.
- Arduino Uno with Dynamixel Shield
- Logic Level Converter to connect the Raspberry Pi 4 and the Arduino Uno
- Pi Zero 2 with Pi Camera

### Schematic

![Schematic](https://github.com/Ivanf1/robot-programming-project/raw/main/assets/schematic.jpg)

### Mecanum wheels motion

![Mecanum](https://github.com/Ivanf1/robot-programming-project/raw/main/assets/mecanum.svg)

### Ros nodes graph

![RosNodeGraph](https://github.com/Ivanf1/robot-programming-project/raw/main/assets/rosgraph.svg)

## Linked repositories

| Repository Name                                                            | Description                                                                   |
| -------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| [robot-motor-controller](https://github.com/Ivanf1/robot-motor-controller) | Code for managing motor control, including speed, direction, and movement.    |
| [robot-ros](https://github.com/Ivanf1/robot-ros)                           | ROS packages for communication, navigation, and sensor integration.           |
| [robot-controller-app](https://github.com/Ivanf1/robot-controller-app)     | A mobile application for remotely controlling the robot.                      |
| [robot-3d-model](https://github.com/Ivanf1/robot-3d-model)                 | 3D models and simulation files for testing the robot in virtual environments. |
