
# Agricultural Vehicle Leader–Follower Control System

## Overview

This project focuses on the development of a leader–follower control system for a hydraulically driven agricultural vehicle in collaboration with Duru Machinery. The work includes mechanical system analysis, STM32-based control hardware design, and ROS 2/Gazebo simulation.

## Agricultural Vehicle

<p align="center">
  <img src="media/agricultural_vehicle_front.png" alt="Front view of agricultural vehicle" width="48%">
  <img src="media/agricultural_vehicle.jpg" alt="Rear view of agricultural vehicle" width="48%">
</p>

## Mechanical System Analysis

Analyzed the hydrostatic transmission (HST) and mechanical linkage connecting the travel lever to the HST control input.

<img src="media/hst.png" alt="HST drive mechanism" width="550">

- Measured actuation torque across the full travel-lever range and at the transmission-side control point.
- Compared potential actuator locations based on mechanical characteristics and installation constraints.
- Selected lever-side actuation to preserve the original mechanical linkage and enable a removable actuator assembly.

## STM32 Control Hardware

Designed and assembled a four-layer STM32-based control PCB to meet the identified automation requirements.

- RS-485 communication interfaces
- Relay outputs for actuator control
- Encoder interface for feedback

<img src="media/stm32_pcb.png" alt="STM32 main control PCB 3D render" width="600">

## ROS 2 / Gazebo Simulation

Adapted existing UWB-based leader–follower control code and evaluated vehicle tracking behavior across simulated turning scenarios in ROS 2/Gazebo.

<img src="media/gazebo_simulation.png" alt="Leader-follower simulation in Gazebo" width="600">

## My Contributions

- Analyzed the hydraulic drive mechanism and measured actuation torque to identify an appropriate actuation point.
- Defined control hardware requirements and designed and assembled the STM32-based main control PCB.
- Adapted leader–follower control code and evaluated tracking behavior in ROS 2/Gazebo.
