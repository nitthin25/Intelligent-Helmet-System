# Intelligent-Helmet-System
IoT-based Intelligent Helmet System using ESP32, ESP32-CAM, GSM and multiple sensors for accident detection, fatigue monitoring, alcohol detection and emergency SMS alerts.

# 🪖 Intelligent Helmet System

> An IoT-based Intelligent Helmet System that enhances rider safety using **ESP32**, **ESP32-CAM**, **GSM communication**, and multiple environmental sensors for real-time accident detection, fatigue monitoring, alcohol detection, and emergency alerts.

![GitHub](https://img.shields.io/badge/ESP32-IoT-red)
![Arduino](https://img.shields.io/badge/Arduino-C++-00979D)
![License](https://img.shields.io/badge/License-MIT-blue)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

# 📖 Overview

Road accidents involving motorcyclists often result in delayed medical assistance due to the inability of riders to seek immediate help after an accident. Driver fatigue, alcohol consumption, and hazardous environmental conditions further increase accident risks.

The **Intelligent Helmet System** is an IoT-based smart safety solution designed to minimize these risks by continuously monitoring the rider and the surrounding environment.

The system automatically detects critical events such as:

- 🚨 Accident Detection
- 😴 Driver Fatigue Detection
- 🍺 Alcohol Detection
- 🌫️ Poor Air Quality Detection
- 🌡️ High Temperature Detection
- 🆘 Manual Emergency Panic Button

Whenever a dangerous situation is detected, the system immediately:

- Activates a local buzzer
- Sends emergency SMS alerts through the GSM network
- Provides continuous monitoring using a non-blocking embedded system architecture

---

# 🚀 Features

- 🚨 Automatic Accident Detection using MPU6050
- 😴 Driver Fatigue Detection using ESP32-CAM
- 🍺 Alcohol Detection using MQ-3 Sensor
- 🌫️ Air Quality Monitoring using MQ-135
- 🌡️ Temperature Monitoring using DHT11
- 📱 Emergency SMS Alerts using SIM800L GSM Module
- 🔔 5-Second Audible Buzzer Alert
- 🆘 Manual Panic Button
- ⚡ Non-blocking Event Driven Programming
- 🔄 Automatic Sensor Calibration
- 🔋 Battery Powered Design
- 🛡️ Dual ESP32 Architecture for Improved Reliability

---

# 🏗️ System Architecture

The project consists of two independent modules.

## Module 1 – Main Safety Hub (ESP32)

Responsible for:

- Accident Detection
- Alcohol Detection
- Air Quality Monitoring
- Temperature Monitoring
- Panic Button Detection
- GSM Communication
- Buzzer Control

---

## Module 2 – Fatigue Detection (ESP32-CAM)

Responsible for:

- Real-time Driver Monitoring
- Motion-Based Fatigue Detection
- Sending Alert Signal to Main Hub

---

# 🧰 Hardware Components

| Component | Purpose |
|------------|----------|
| ESP32 | Main Controller |
| ESP32-CAM | Driver Fatigue Detection |
| MPU6050 | Crash Detection |
| MQ-3 | Alcohol Detection |
| MQ-135 | Air Quality Monitoring |
| DHT11 | Temperature Monitoring |
| SIM800L | GSM SMS Communication |
| Active Buzzer | Local Alert |
| Panic Button | Manual Emergency Alert |
| Li-Ion Battery | Power Supply |
| TP4056 Charging Module | Battery Charging |

---

# ⚙️ Working Principle

1. The ESP32 continuously monitors all connected sensors.

2. The ESP32-CAM independently performs fatigue detection.

3. If any hazardous condition is detected, such as:

- Accident
- Driver Fatigue
- Alcohol Detection
- Poor Air Quality
- High Temperature
- Panic Button Press

the system immediately:

- Activates the buzzer
- Sends an emergency SMS
- Continues monitoring without blocking other tasks

---

# 📂 Repository Structure

```
Intelligent-Helmet-System/

│
├── Main_Hub_Code/
│      Main_Hub.ino
│
├── ESP32_CAM_Code/
│      Fatigue_Detection.ino
│
├── Circuit_Diagrams/
│
├── Images/
│
├── Documents/
│      Project_Report.pdf
│      Presentation.pdf
│
├── Libraries_Required.md
│
├── README.md
│
└── LICENSE
```

---

# 🔌 Pin Connections

| Device | ESP32 Pin |
|----------|-----------|
| MPU6050 SDA | GPIO 21 |
| MPU6050 SCL | GPIO 22 |
| DHT11 | GPIO 4 |
| MQ-3 | GPIO 35 |
| MQ-135 | GPIO 34 |
| Panic Button | GPIO 15 |
| Buzzer | GPIO 5 |
| SIM800L TX | GPIO 26 |
| SIM800L RX | GPIO 27 |
| ESP32-CAM Alert Pin | GPIO 13 |

---

# 📚 Required Arduino Libraries

Install the following libraries before uploading the code.

- Wire
- WiFi
- DHT Sensor Library
- Adafruit MPU6050
- Adafruit Unified Sensor
- TinyGSM
- ESP32 Board Package

---

# 💻 Software Used

- Arduino IDE
- ESP32 Board Package
- C++
- Embedded C
- ESP32 Camera Library

---

# 📸 Project Demonstration

## Prototype

<img width="536" height="370" alt="Image" src="https://github.com/user-attachments/assets/db1b6a63-c6a5-4453-ba03-27d22cf28169" />

---

## Hardware Setup

> *(Insert Hardware Setup Image Here)*

---

## Serial Monitor

> *(Insert Serial Monitor Screenshot Here)*

---

## Fatigue Detection Interface

> *(Insert ESP32-CAM Screenshot Here)*

---

# 🔄 System Workflow

```
Helmet Powered ON
        │
        ▼
Initialize Sensors
        │
        ▼
Sensor Calibration
        │
        ▼
Continuous Monitoring
        │
        ▼
 ┌──────────────────────────────┐
 │ Accident Detected            │
 │ Fatigue Detected             │
 │ Alcohol Detected             │
 │ High Temperature             │
 │ Poor Air Quality             │
 │ Panic Button                 │
 └──────────────┬───────────────┘
                │
                ▼
      Trigger Emergency Alert
                │
       ┌────────┴────────┐
       ▼                 ▼
 Activate Buzzer    Send SMS
```

---

# 🎯 Applications

- Smart Helmets
- Rider Safety Systems
- Accident Detection
- Fleet Monitoring
- Emergency Alert Systems
- Intelligent Transportation Systems
- IoT Safety Solutions

---

# 🔮 Future Improvements

- GPS Location Tracking
- Mobile Application
- Cloud-Based Monitoring Dashboard
- AI-Based Fatigue Detection
- PCB Design for Compact Integration
- Rechargeable Smart Helmet
- Live Location Sharing
- Emergency Contact Management

---

# 📊 Technologies Used

- ESP32
- ESP32-CAM
- Arduino
- Embedded C++
- IoT
- Computer Vision
- GSM Communication
- Sensor Fusion

---

# 👨‍💻 Authors

**Nitthin M M**

B.Tech Electronics and Communication Engineering

SRM Institute of Science and Technology



# 📄 License

This project is released under the MIT License.

Feel free to use, modify, and improve this project for educational and research purposes.

---

# ⭐ Support

If you found this project helpful, please consider giving it a **⭐ Star** on GitHub!

It motivates us to build more innovative IoT and Embedded Systems projects.
