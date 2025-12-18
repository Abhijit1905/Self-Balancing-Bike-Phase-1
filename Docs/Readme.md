# Self-Balancing Bike using PID Control and IMU-6050

This repository contains the design, simulation, and control implementation of a
self-balancing two-wheeled bike. The system uses a PID control algorithm with real-time
orientation feedback from an IMU-6050 sensor to maintain balance. Mechanical design was
developed in SolidWorks and validated through dynamic simulation in CoppeliaSim before
hardware implementation.

---

## Project Overview

Maintaining balance in a two-wheeled system is a classic control systems problem involving
an unstable, underactuated dynamic system. This project focuses on stabilizing a bike-like
structure by continuously measuring tilt angle and applying corrective actions through a
PID controller.

The project follows a simulation-driven development approach, where the mechanical
design and control logic were first tested in a virtual environment before deployment on
hardware.

---

## System Architecture

- IMU-6050 for tilt angle and angular velocity measurement
- Microcontroller-based control unit
- PID control loop for balance correction
- Actuators for counteracting tilt
- SolidWorks-designed mechanical chassis
- CoppeliaSim-based dynamic simulation

---

## Simulation

The complete system was simulated using **CoppeliaSim** to analyze:
- Tilt response and recovery behavior
- Controller stability and tuning
- Effect of disturbances on balance
- Dynamic interaction between chassis and actuators

Simulation helped refine PID gains and reduce hardware trial-and-error.

---

## Sensor Calibration

Accurate IMU calibration was essential for stable operation. The following steps were
implemented:
- Gyroscope bias and drift compensation
- Accelerometer offset correction
- Noise reduction using filtering techniques
- Angle estimation using sensor fusion

---

## Control Strategy

A classical **PID controller** was implemented to minimize tilt error:
- **Proportional (P):** Immediate correction based on tilt error
- **Integral (I):** Eliminates steady-state error
- **Derivative (D):** Predictive damping to reduce oscillations

PID parameters were tuned iteratively using simulation and experimental testing.

---

## Tools & Technologies

- SolidWorks (Mechanical Design)
- CoppeliaSim (Dynamic Simulation)
- Arduino / Microcontroller Platform
- IMU-6050 (Gyroscope + Accelerometer)
- Embedded C / C++
- PID Control Theory

---

## Repository Structure


