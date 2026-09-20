# 2-DOF Bilateral Manipulator 3D Models

This repository provides the STL files for the two-link local and remote manipulators used in the experimental bilateral control system presented in:

**"Synchronization of Bilateral Control Systems Using Time Delay Compensation-Based Sliding Mode Control."**

The files are provided to facilitate reproduction of the experimental hardware platform.

## Experimental Platform

The bilateral control system consists of two 2-DOF planar manipulators: a local manipulator and a remote manipulator.

Each actuated joint uses a **ROBOTIS DYNAMIXEL PM42-010-S260-R** actuator. The joint positions are measured using the integrated motor encoders, and the motors are interfaced with **OpenCR** microcontroller units.

Communication between the local and remote manipulators and computation of the control inputs are implemented using **MATLAB/Simulink** and the **Robot Operating System (ROS)**.

The control system is operated with a sampling period of **0.02 s**.

## Actuator

The actuator used for each joint is the **ROBOTIS DYNAMIXEL PM42-010-S260-R**.

Main manufacturer specifications are:

| Specification | Value |
|---|---|
| Input voltage | 24.0 V |
| Communication | RS-485 |
| Gear ratio | 257.019:1 |
| Resolution | 526,374 pulse/rev |
| Continuous torque | 1.7 N·m |
| Continuous speed | 26.0 rev/min |
| Weight | 270 g |
| Dimensions | 42 × 72 × 42 mm |

## 3D Model Files

The STL files included in this repository correspond to the 3D-printable mechanical components of the manipulators used in the experiments.

These files can be used to reproduce the mechanical structure of the experimental platform.

## Basic Assembly

1. 3D-print the required STL parts.
2. Install the PM42-010-S260-R actuators at the manipulator joints.
3. Assemble the printed links to construct the two-link manipulator.
4. Repeat the assembly for the local and remote manipulators.
5. Connect the joint actuators to the OpenCR-based control hardware.
6. Obtain the joint-position measurements from the motor encoders.

## Notes

- The STL files correspond to the manipulator hardware used in the experiments.
- Printing tolerances may need to be adjusted depending on the 3D printer and printing conditions.
- The PM42-010-S260-R uses RS-485 communication.
- The experimental control implementation was developed using MATLAB/Simulink and ROS.

## Related Work

These 3D models are provided as supplementary material for the experimental platform used in:

**Synchronization of Bilateral Control Systems Using Time Delay Compensation-Based Sliding Mode Control**
