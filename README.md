# Automated Water Tank System

This repository contains the implementation of an automated water tank system, designed to minimize water waste, reduce energy consumption, and optimize the efficiency of water pumps through PID-controlled water level sensing and servo motor actuation.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [System Overview](#system-overview)
- [Components](#components)
- [Experiments and Results](#experiments-and-results)

## Introduction
In Lebanon, water tanks on rooftops are critical, often more essential than electricity. The automated water tank system addresses issues of water scarcity and inefficiency in water management, particularly in regions with unreliable water supply and frequent power outages. This project aims to implement a smart water control system that uses sensors to monitor water levels and adjust pump activity accordingly.

## Features
- **Real-time Water Level Monitoring**: Uses ultrasonic sensors to measure water levels accurately.
- **Automated Water Pump Control**: Adjusts the power output of the water pump based on real-time data to minimize waste and optimize energy usage.
- **User-Friendly Interface**: Displays water levels and estimated refill times on an LCD screen.
- **Cost Savings**: Reduces water and electricity bills by preventing overfilling and optimizing pump operation.

## System Overview
The system includes:
- Sensors for accurate water level measurement.
- Servo motors for precise control of water flow.
- An LCD display for real-time monitoring.
- A control algorithm (PID and Fuzzy Logic) to manage the system efficiently.

## Components
- **Ultrasonic Sensor**: Measures the distance to the water surface.
- **Servo Motor**: Controls the opening and closing of water valves.
- **LCD Display**: Shows real-time data about water levels and system status.
- **Control Unit**: Implements PID and Fuzzy Logic controllers for system regulation.

## Experiments and Results
The system was tested using both PID and Fuzzy Logic controllers. The results showed that the Fuzzy Logic controller performed better in terms of maintaining stable water levels with minimal overshoot and steady-state error.

### PID Controller
- Initial tuning parameters: `kp=0.6`, `ki=0.02`, `kd=1.8`
- The PID controller struggled with maintaining stable water levels and showed poor performance.

### Fuzzy Logic Controller
- Implemented using five rules.
- Demonstrated better performance in maintaining desired water levels with minimal error.

