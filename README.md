
# Agricultural Vehicle Leader–Follower Control System

## Overview

This project focuses on developing a leader–follower control system for a hydraulically driven agricultural vehicle in collaboration with Duru Machinery. The work includes mechanical and electrical system analysis, lever-actuation mechanism design, STM32-based control hardware, and ROS 2/Gazebo simulation.

## Agricultural Vehicle

<p align="center">
  <img src="media/agricultural_vehicle_front.png" alt="Front view of agricultural vehicle" width="48%">
  <img src="media/agricultural_vehicle.jpg" alt="Rear view of agricultural vehicle" width="48%">
</p>

## Mechanical & Electrical System Analysis

Analyzed the hydrostatic transmission (HST), the mechanical linkage connecting the travel lever to the HST control input, and the vehicle's existing electrical control signals.

<img src="media/hst.png" alt="HST drive mechanism" width="550">

- Measured actuation torque at the travel lever and HST-side control input, and examined forward/reverse lever operation.
- Characterized voltage levels and signal states associated with engine starting and steering.
- Compared candidate actuation points while considering mechanical characteristics and installation constraints.

## Actuator & Linkage Design

Selected lever-side actuation to preserve the original mechanical linkage and support removable installation.

- Estimated actuator thrust requirements based on the measured peak lever force and linkage geometry.
- Selected a linear actuator and designed a linkage assembly to meet the actuation requirements.
- Installed the actuator linkage and verified actuator-driven lever movement with the engine off.

<img src="media/lever_actuator.jpg" alt="Linear actuator and linkage mounted to the travel lever" width="600">

## STM32 Control Hardware

Designed and assembled a four-layer STM32-based control PCB to meet the identified automation requirements.

- RS-485 communication interfaces
- Relay-based steering control
- Motor driver interface for travel-lever actuator control
- Encoder interface for actuator position feedback

<img src="media/stm32_pcb.png" alt="STM32 main control PCB 3D render" width="600">

## ROS 2 / Gazebo Simulation

Adapted existing UWB-based leader–follower control code and evaluated vehicle tracking behavior across simulated turning scenarios in ROS 2/Gazebo.

<img src="media/gazebo_simulation.png" alt="Leader-follower simulation in Gazebo" width="600">

## My Contributions

- Analyzed the HST drive mechanism and electrical control signals, and measured actuation torque to select an appropriate actuation point.
- Developed the lever-actuation mechanism and designed and assembled the STM32-based main control PCB.
- Adapted existing leader–follower control code and evaluated tracking behavior in ROS 2/Gazebo.
