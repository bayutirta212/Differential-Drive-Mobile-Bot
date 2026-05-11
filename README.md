# Differential Drive Bot PCB

Custom PCB design for a compact Differential Drive Robot using ESP32 DevKit V1 (30 Pin).

## Features

- Dual motor differential drive system
- Encoder feedback support
- OLED display integration
- Ultrasonic obstacle detection
- GPIO expansion using multiplexer
- Line tracking sensor support
- Compact PCB layout
- ESP32-based control system

---

# Hardware Components

- ESP32 DevKit V1 (30 Pin)
- JGA12 N20 Motor Encoder
- DRV8833 Dual Motor Driver
- HC-SR04 Ultrasonic Sensor
- SSD1306 OLED Display
- CD74HC4067 16-Channel Multiplexer
- TCRT5000 IR Reflective Sensor

---

# System Overview

This robot uses a differential drive mechanism where each wheel is independently controlled using the DRV8833 motor driver.

The ESP32 handles:
- Motor control
- Encoder reading
- OLED communication
- Ultrasonic sensing
- Multiplexer control
- Sensor data processing

The CD74HC4067 multiplexer is used to expand input capability while minimizing GPIO usage.

---

# Pin Configuration

## DRV8833 Motor Driver

| ESP32 Pin | Function |
|---|---|
| GPIO16 | Motor A IN1 |
| GPIO17 | Motor A IN2 |
| GPIO05 | Motor B IN1 |
| GPIO23 | Motor B IN2 |

---

## Motor Encoder

| ESP32 Pin | Function |
|---|---|
| GPIO39 | Left Encoder A |
| GPIO36 | Left Encoder B |
| GPIO35 | Right Encoder A |
| GPIO34 | Right Encoder B |

---

## HC-SR04

| ESP32 Pin | Function |
|---|---|
| GPIO19 | Trigger |
| GPIO18 | Echo |

---

## SSD1306 OLED (I2C)

| ESP32 Pin | Function |
|---|---|
| GPIO21 | SDA |
| GPIO22 | SCL |

---

## CD74HC4067 Multiplexer

| ESP32 Pin | Function |
|---|---|
| GPIO27 | S0 |
| GPIO26 | S1 |
| GPIO25 | S2 |
| GPIO33 | S3 |
| GPIO32 | SIG |
| GIPO13 | EN |

---


# Repository Contents

- Schematic files
- PCB layout files
- Gerber files
- 3D PCB preview
- Wiring references

---

# Software Compatibility

This project can be programmed using:
- Arduino IDE
- PlatformIO

Recommended Libraries:
- Adafruit SSD1306
- Adafruit GFX
- ESP32Encoder
- NewPing

---

# Applications

- Line follower robot
- Obstacle avoidance robot
- Autonomous mobile robot
- Educational robotics platform

---


# Future Improvements

- IMU integration
- Battery monitoring
- PID motor control
- WiFi telemetry
- ROS compatibility

---

# License

This project is open-source under the MIT License.

---

# Author

Rafael Subally  
Student at Mechatronics Engineering Education  
Universitas Negeri Yogyakarta
