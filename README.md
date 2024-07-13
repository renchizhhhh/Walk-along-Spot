# Walk-along-Spot

## Overview

This repository contains the source code and implementation details for an experiment comparing two hands-free methods for directing mobile robots: voice control and gesture control. These methods were tested in two settings: with the human stationary and walking freely. The experiment was conducted using the quadrupedal robot Spot from Boston Dynamics, controlled via a combination of ROS and Unity with the HoloLens 2 interface.

## Repository Structure

This repository is organized into two submodules, each containing essential components for the experiment:

### 1. SpotDockerImage

The `SpotDockerImage` submodule contains a Catkin workspace designed to control Spot from Boston Dynamics. It uses internal odometry to determine the 6D position of Spot. The code can run in Docker or on Windows with a ROS installation.

#### Key Features:
- ROS nodes for connecting and controlling Spot.
- State machine for serialized execution of actions.

### 2. Unity-MRTK-ROS-Spot-NUI

The `Unity-MRTK-ROS-Spot-NUI` submodule provides a Unity implementation that allows control of the robot using Microsoft HoloLens 2. This is achieved by creating a natural user interface using speech, gestures, and gaze.

#### Key Features:
- Communication with ROS nodes to control the robot.
- Customizable messages for robot control.
- Integration of Mixed Reality Toolkit for HoloLens 2.

## Getting Started

To clone this repository along with its submodules, use the following command:

```bash
git clone --recurse-submodules <repository-url>
```

After cloning, follow the setup instructions provided in each submodule's README file to set up your development environment and run the experiment.

## What You Will Find in the Paper

The paper accompanying this repository provides a detailed analysis of the experiment, including:
- Methodology for comparing voice and gesture control methods.
- Participant setup and experimental design.
- Data analysis and results of the intuitiveness and preferences of the participants.
- Detailed discussion on the impact of walking on stimulus-response compatibility.
- Conclusions and recommendations for enhancing gesture control effectiveness.

## What You Will Find in the Submodules

### SpotDockerImage
- Instructions for setting up and running the ROS nodes.
- Docker setup for controlling Spot.
- State machine implementation for action control.

### Unity-MRTK-ROS-Spot-NUI
- Unity project setup for HoloLens 2.
- Implementation of the natural user interface using speech, gestures, and gaze.
- Communication setup between Unity and ROS nodes.

## Contact

For any questions or further information, please leave an issue and I will try to help! This will help people facing the same questions in the future. 

## License

This project is released under a [MIT License](#license). Feel free to use, modify, and distribute any of the contents of this repository in accordance with the license specifications.

We hope the OpenChessRobot serves as a valuable tool for your research and development in human-robot interaction. Happy experimenting!

## Copyright Notice:
Technische Universiteit Delft hereby disclaims all copyright interest in the program “OpenChessBot: An Open-Source Reproducible Chess Robot for Human-Robot Interaction Research” written by the Author(s). 

© 2024, [Renchi Zhang], [Paper_to_add]
