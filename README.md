# Neo Pilot E2E (End-to-end)

**Thesis Title: Small-Scale Autonomous Car: Design, Implementation, and Remote Monitoring**

**Neo Pilot E2E** is my B.Sc. thesis project in Electrical Engineering. The project focuses on designing, implementing, and testing a small-scale autonomous car with computer vision, end-to-end learning, embedded deployment, and remote monitoring.

The final system was deployed on an **NVIDIA Jetson Nano** and tested on a physical test track.


## Overview

This project studies and implements different approaches for autonomous navigation in a small-scale vehicle. The work was developed around the rules and constraints of small autonomous car competitions such as the FIRA autonomous car league.

The project includes:
- A small-scale autonomous vehicle platform
- Camera-based perception
- Classical computer vision pipelines
- End-to-end neural-network-based steering prediction
- Sensor integration
- Embedded deployment on Jetson Nano
- A remote monitoring and control center
- Test-track design and real-world evaluation

## Thesis Context

This repository is connected to my bachelor thesis:
**Small-Scale Autonomous Car: Design, Implementation, and Remote Monitoring**

The thesis investigates the design of a complete autonomous navigation system, from hardware selection and vehicle assembly to software implementation, perception, control, data collection, model training, deployment, and testing.
The original thesis document is written in Persian, but this README provides an English summary of the project, methods, and implementation.

## System Architecture

The project was developed using two main autonomous navigation paradigms.

### 1. Modular Navigation

The modular approach separates the autonomous driving task into multiple components:
- Image preprocessing
- Lane and line detection
- Road sign and guide sign detection
- Obstacle detection
- Intersection and turn detection
- PID-based steering/control logic
- Simulation and real-world deployment

### 2. End-to-End Learning

The end-to-end approach uses a neural network to predict steering commands directly from camera input.

The pipeline includes:
- Manual driving and data collection
- Image preprocessing
- Dataset preparation
- Neural network model design
- Model training
- Testing on collected data
- Deployment on Jetson Nano
- Real-world test-track evaluation

## Hardware

The autonomous car platform used several embedded and sensing components, including:
- NVIDIA Jetson Nano as the main processing board
- Camera module for visual perception
- Ultrasonic sensor for obstacle sensing
- GPS module
- Arduino Uno for low-level control
- DC motors with gearbox
- Servo motor for steering
- Motor driver
- Power bank and Li-ion battery system
- Custom small-scale vehicle chassis

## Software

The software stack included:
- Python
- OpenCV
- PyTorch
- SQLite
- Flask
- WebSocket communication
- HTML, CSS, and JavaScript for the monitoring interface
- Embedded Linux deployment on Jetson Nano

## Computer Vision and AI Components

The project includes several perception and learning components:

- Image grayscale conversion
- Cropping and region-of-interest selection
- CLAHE preprocessing
- Thresholding
- Edge detection
- Contour detection
- Lane and line detection
- Road sign detection
- End-to-end neural network training
- Steering angle prediction
- Real-time inference on embedded hardware

## Remote Monitoring and Control Center

A web-based command center was developed to monitor the vehicle during operation.

The monitoring system included:

- Data collection and storage
- Client-server communication
- WebSocket-based real-time updates
- Backend and frontend implementation
- Remote access to vehicle status and collected information

## Deployment

The trained and implemented navigation system was deployed on the Jetson Nano and tested on a designed physical test track.

The deployment process included:

- Installing and configuring the Jetson Nano environment
- Connecting the camera and sensors
- Running perception and control software on embedded hardware
- Integrating the vehicle hardware and software
- Testing autonomous driving behavior on the track

## Visuals

### Jetson Nano

<img src="./imgs/jetson.png" width="400px">

### Vehicle Prototype

<img src="./imgs/car.jpg" width="400px">

### Demo, Test on the test track:

<img src="./imgs/demo0_e2e.gif" width="400px">

### End-to-End Model / Training

_Add image or training curve here._

### Remote Monitoring Interface

_Add screenshot here._

## Project Status

The project successfully implemented a complete small-scale autonomous vehicle prototype, including perception, control, embedded deployment, and remote monitoring. The system was tested on a physical track with reduced human intervention.

## Keywords

Autonomous driving, small-scale autonomous car, computer vision, deep learning, end-to-end learning, steering prediction, Jetson Nano, embedded AI, robotics, remote monitoring, PyTorch, OpenCV.
