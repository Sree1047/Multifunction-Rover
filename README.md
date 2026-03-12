🤖 Multifunction Rover – IoT Smart Surveillance Robot










A Multifunction IoT Rover designed for remote exploration, obstacle detection, and live video monitoring.
This rover integrates Arduino Uno, ESP32-CAM, Bluetooth communication, ultrasonic sensors, and solar power to create a compact smart robotic system.

The project demonstrates the integration of robotics, embedded systems, and Internet of Things (IoT) technologies.

📖 Table of Contents

Project Overview

System Features

Hardware Components

System Architecture

Hardware Connections

ESP32-CAM Video Streaming

Software Requirements

Project Structure

Installation & Setup

Working Principle

Future Improvements

Team Members

🚀 Project Overview

The Multifunction Rover is a four-wheel robotic vehicle that can be controlled through Bluetooth commands or voice commands via mobile application.

The rover also performs automatic obstacle avoidance and provides real-time live video streaming using ESP32-CAM.

Key capabilities include:

• Remote rover control
• Autonomous obstacle detection
• Wireless video streaming
• Voice command navigation
• Solar powered charging system

This system can be used in:

Surveillance robots

Disaster monitoring

Remote exploration

Educational robotics projects

⭐ System Features
Remote Control

Control rover movement using Bluetooth mobile application.

Voice Command Control

The rover can receive voice instructions from mobile apps.

Obstacle Avoidance

An ultrasonic sensor and servo motor detect obstacles and guide the rover safely.

Live Video Streaming

The ESP32-CAM module streams real-time video over WiFi.

Solar Charging

A 6V solar panel and TP4056 module recharge the battery.

🧰 Hardware Components
Component	Description
Arduino Uno R3	Main microcontroller
ESP32-CAM	Live video camera module
L298N Motor Driver	Controls DC motors
Ultrasonic Sensor (HC-SR04)	Detects obstacles
Servo Motor	Rotates ultrasonic sensor
HC-06 Bluetooth Module	Wireless communication
Solar Panel (6V)	Power generation
TP4056 Charging Module	Battery charging
18650 Li-ion Battery	Power supply
LED & Resistors	Status indication
Robot Chassis	Frame with motors
Jumper Wires	Electrical connections
🏗 System Architecture
            Mobile App
        (Bluetooth Control)
                 │
                 ▼
          HC-06 Bluetooth
                 │
                 ▼
            Arduino Uno
                 │
        ┌────────┴────────┐
        ▼                 ▼
   Motor Driver      Ultrasonic Sensor
      (L298N)             │
        │                 ▼
        ▼             Servo Motor
     DC Motors            │
        │                 ▼
        └──── Rover Navigation ────┘
Video Streaming System
ESP32-CAM
   │
   ▼
WiFi Network
   │
   ▼
Mobile / Laptop Browser
   │
   ▼
Live Camera Stream
🔌 Hardware Connections
L298N Motor Driver
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

To upload code to the ESP32-CAM, connect it with an FTDI programmer.

ESP32-CAM	FTDI
5V	VCC
GND	GND
U0R	TX
U0T	RX
IO0	GND (for upload mode)

After uploading code:

Disconnect IO0 from GND

Press RESET

The camera will start streaming.

💻 Software Requirements

Arduino IDE

ESP32 Board Package

USB Drivers

Android Bluetooth Controller App

Serial Monitor  


⚙️ Installation & Setup
1 Install Arduino IDE

Download and install Arduino IDE.

2 Upload Arduino Code

Upload the rover control program to Arduino Uno.

3 Upload ESP32-CAM Code

Upload camera streaming code using FTDI programmer.

4 Power the Rover

Insert 18650 Li-ion battery and switch ON.

5 Connect Bluetooth

Pair mobile with HC-06 module.

6 Open Mobile App

Control rover using buttons or voice commands.

7 Open Camera Stream

Open browser and enter:

http://ESP32_IP_ADDRESS
⚡ Working Principle

Mobile app sends commands via Bluetooth

Arduino receives commands through HC-06 module

Motor driver controls rover movement

Ultrasonic sensor detects obstacles

Servo motor scans left and right directions

Rover avoids obstacles automatically

ESP32-CAM streams real-time video via WiFi

Solar panel charges the battery

🔮 Future Improvements

GPS navigation system

AI object detection

Night vision camera

Autonomous path planning

Cloud IoT monitoring

Mobile app integration with video feed
