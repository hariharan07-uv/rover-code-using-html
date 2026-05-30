# ESP32 WiFi Controlled Rover

## Overview

ESP32 WiFi Controlled Rover is a browser-controlled robotic vehicle designed using ESP32 and dual DC motors. The robot connects to a WiFi network and hosts an embedded web server that provides a real-time control dashboard accessible from any smartphone, tablet, or computer.

The web interface allows users to control movement direction and motor speed wirelessly without requiring a dedicated mobile application.

This project demonstrates wireless robotics, embedded systems, web server development, motor control, and IoT-based remote operation.

---

# Features

## Wireless Robot Control

* WiFi-based communication
* Browser-accessible dashboard
* No mobile application required
* Real-time control

## Motion Control

Supported commands:

* Forward
* Reverse
* Left Turn
* Right Turn
* Stop

## Speed Control

* PWM motor control
* Adjustable speed levels
* Real-time updates
* Smooth acceleration

## Embedded Web Server

* Hosted directly on ESP32
* Lightweight interface
* Mobile friendly design

---

# Hardware Components

| Component                      | Quantity |
| ------------------------------ | -------- |
| ESP32 Development Board        | 1        |
| L298N / TB6612FNG Motor Driver | 1        |
| DC Gear Motors                 | 2        |
| Robot Chassis                  | 1        |
| Battery Pack                   | 1        |
| Wheels                         | 2        |
| Castor Wheel                   | 1        |

---

# System Architecture

User Device
↓
Web Browser
↓
WiFi Network
↓
ESP32 Web Server
↓
Motor Driver
↓
DC Motors
↓
Robot Movement

---

# Pin Configuration

## Motor A

| Function | ESP32 GPIO |
| -------- | ---------- |
| IN1      | GPIO27     |
| IN2      | GPIO26     |
| PWM      | GPIO15     |

---

## Motor B

| Function | ESP32 GPIO |
| -------- | ---------- |
| IN1      | GPIO33     |
| IN2      | GPIO25     |
| PWM      | GPIO32     |

---

# WiFi Configuration

SSID:

Abcd

Password:

123456789

Update these credentials according to your network before deployment.

---

# Web Dashboard Features

### Movement Controls

* FORWARD
* LEFT
* RIGHT
* REVERSE
* STOP

### Speed Controller

* Adjustable slider
* Range: 0 – 100%
* Real-time PWM adjustment

---

# Working Principle

### Forward Motion

Both motors rotate forward.

### Reverse Motion

Both motors rotate backward.

### Left Turn

Left motor reverses while right motor moves forward.

### Right Turn

Right motor reverses while left motor moves forward.

### Stop

Both motors are disabled.

---

# PWM Speed Control

Motor speed is controlled using:

* PWM Frequency: 30 kHz
* Resolution: 8-bit

Speed values selected through the browser slider are converted into PWM duty cycles and applied to both motors.

---

# Software Libraries

Required Libraries:

* WiFi.h
* WebServer.h
* ESP32 Arduino Core

---

# Installation

## Step 1

Install ESP32 Board Package in Arduino IDE.

## Step 2

Open the project.

## Step 3

Update WiFi credentials.

## Step 4

Upload code to ESP32.

## Step 5

Power the robot.

## Step 6

Open Serial Monitor.

Example:

WiFi connected.
IP address:
192.168.1.120

## Step 7

Open the displayed IP address in a browser.

---

# Applications

* Surveillance Robot
* Inspection Rover
* Educational Robotics
* Wireless Robot Control
* Smart Mobility Research
* IoT Demonstrations
* Remote Navigation Systems

---

# Future Improvements

* ESP32 Camera Integration
* Live Video Streaming
* Obstacle Avoidance
* Voice Control
* Mobile Application
* GPS Navigation
* Autonomous Driving
* MQTT Cloud Dashboard
* AI Object Tracking

---

# Project Highlights

✔ ESP32 Based

✔ WiFi Controlled

✔ Embedded Web Server

✔ PWM Motor Control

✔ Browser-Based Dashboard

✔ Wireless Navigation

✔ Real-Time Speed Adjustment

✔ Expandable Architecture

---

# Author

Hariharan Balakrishnan

B.E Electronics and Communication Engineering

Embedded Systems | Robotics | IoT | Edge AI | ESP32 | Zephyr RTOS
