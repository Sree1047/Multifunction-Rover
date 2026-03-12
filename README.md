🤖 Multifunction Rover – IoT Smart Surveillance Robot












📊 GitHub Project Statistics

📖 Table of Contents

Abstract

Project Overview

Key Features

Hardware Components

System Architecture

Hardware Connections

ESP32-CAM Video Streaming

Project Images

Live Demo

Installation

Working Principle

Future Scope

Research Contribution

Project Structure

Team Members

🧠 Abstract

Rovers play an important role in remote exploration, surveillance, and scientific analysis.
This project presents a Multifunction IoT Rover capable of performing multiple robotic tasks including:

Remote navigation

Obstacle detection

Voice command control

Real-time video monitoring

The rover integrates Arduino Uno for motion control and ESP32-CAM for wireless video streaming. A solar-powered charging system improves energy efficiency and sustainability.

This project demonstrates the integration of embedded systems, robotics, and IoT communication technologies to build an intelligent robotic platform.

🚀 Project Overview

The Multifunction Rover is a four-wheel robotic vehicle designed for wireless control and autonomous navigation.

The rover can be operated through:

📱 Bluetooth Mobile Application
🎤 Voice Commands
🤖 Autonomous Obstacle Avoidance Mode

Additionally, the ESP32-CAM module provides live video streaming through WiFi, enabling remote monitoring.

Applications

Security surveillance robots

Disaster response robots

Military reconnaissance

Educational robotics research

⭐ Key Features

✅ Bluetooth Controlled Rover
✅ Voice Command Navigation
✅ Real-time Video Streaming (ESP32-CAM)
✅ Obstacle Detection and Avoidance
✅ Servo-based scanning system
✅ Autonomous navigation
✅ Solar-powered charging system

🧰 Hardware Components
Component	Description
Arduino Uno R3	Main microcontroller
ESP32-CAM	Wireless video camera
L298N Motor Driver	Controls DC motors
Ultrasonic Sensor (HC-SR04)	Detects obstacles
Servo Motor	Rotates ultrasonic sensor
HC-06 Bluetooth Module	Wireless communication
Solar Panel (6V)	Generates power
TP4056 Charging Module	Battery charging module
18650 Li-ion Battery	Power supply
LED & Resistors	Status indicators
Robot Chassis	Mechanical body
🛰 System Architecture
Mobile App / Voice Commands
            │
            ▼
       Bluetooth (HC-06)
            │
            ▼
        Arduino Uno
            │
   ┌────────┴────────┐
   ▼                 ▼
Motor Driver      Ultrasonic Sensor
 (L298N)               │
   │                   ▼
   ▼               Servo Motor
DC Motors               │
   │                    ▼
 Rover Movement     Obstacle Detection
Camera Streaming Architecture
ESP32-CAM
   │
   ▼
WiFi Network
   │
   ▼
Mobile / Laptop Browser
   │
   ▼
Live Video Streaming
🔌 Hardware Connections
Motor Driver (L298N)
L298N	Arduino
ENA	10
IN1	9
IN2	8
IN3	7
IN4	6
ENB	5
Bluetooth Module (HC-06)
HC-06	Arduino
VCC	5V
GND	GND
RX	Pin 3
TX	Pin 2
Ultrasonic Sensor
Sensor	Arduino
VCC	5V
GND	GND
Echo	A2
Trigger	A3
Servo Motor
Servo	Arduino
Signal	A4
VCC	5V
GND	GND
📷 ESP32-CAM Programming Connections

To upload code to ESP32-CAM, use an FTDI programmer.

ESP32-CAM	FTDI
5V	VCC
GND	GND
U0R	TX
U0T	RX
IO0	GND (Upload Mode)

After uploading code:

1️⃣ Disconnect IO0 from GND
2️⃣ Press RESET
3️⃣ Open browser with ESP32 IP address

📸 Project Images

Add rover images to the Images folder.

Rover Model
![Rover Image](Images/rover_model.jpg)
Circuit Diagram
![Circuit Diagram](Images/circuit_diagram.png)
🎥 Live Demo

Add your YouTube project demo.

https://youtu.be/YOUR_VIDEO_LINK

Embed preview:

[![Watch Demo](https://img.youtube.com/vi/YOUR_VIDEO_ID/0.jpg)](https://youtu.be/YOUR_VIDEO_ID)
💻 Software Requirements

Arduino IDE

ESP32 Board Package

Android Bluetooth Controller App

FTDI Programmer

USB Drivers

⚙ Installation & Setup
Step 1

Install Arduino IDE

Step 2

Upload rover control code to Arduino Uno

Step 3

Upload ESP32-CAM streaming code

Step 4

Insert 18650 battery

Step 5

Connect mobile with HC-06 Bluetooth

Step 6

Open camera stream in browser

http://ESP32_IP_ADDRESS
⚡ Working Principle

1️⃣ User sends command through mobile app
2️⃣ Bluetooth module receives command
3️⃣ Arduino processes instructions
4️⃣ Motor driver controls rover motors
5️⃣ Ultrasonic sensor scans environment
6️⃣ Servo motor rotates sensor to detect obstacles
7️⃣ Rover changes direction automatically
8️⃣ ESP32-CAM streams live video through WiFi

🔮 Future Scope

AI object detection using computer vision

GPS navigation system

Autonomous path planning

Cloud-based IoT monitoring

Night vision camera integration

Mobile app with integrated video streaming

🧠 Research Contribution

This project demonstrates the integration of IoT communication with embedded robotics systems.

The rover design improves:

Energy efficiency

Remote monitoring capability

Navigation safety

The platform can be extended for autonomous robotic exploration and surveillance applications.
