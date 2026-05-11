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
| GPIO25 | Motor A IN1 |
| GPIO26 | Motor A IN2 |
| GPIO27 | Motor B IN1 |
| GPIO14 | Motor B IN2 |

---

## Motor Encoder

| ESP32 Pin | Function |
|---|---|
| GPIO34 | Left Encoder A |
| GPIO35 | Left Encoder B |
| GPIO32 | Right Encoder A |
| GPIO33 | Right Encoder B |

---

## HC-SR04

| ESP32 Pin | Function |
|---|---|
| GPIO5 | Trigger |
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
| GPIO19 | S0 |
| GPIO23 | S1 |
| GPIO12 | S2 |
| GPIO13 | S3 |
| GPIO4 | SIG |

---

## TCRT5000

| ESP32 Pin | Function |
|---|---|
| GPIO15 | Sensor Output |

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
- ESP-IDF

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

# Preview

Add your images here:

```md
![Schematic](images/schematic.png)
![PCB Front](images/pcb_front.png)
![PCB Back](images/pcb_back.png)
```

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
Mechatronics Engineering Education  
Universitas Negeri Yogyakarta
