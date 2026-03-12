🤖 Multifunction Rover – IoT Smart Surveillance Robot

------------------------------------------




📖 Project Overview

The Multifunction Rover is an IoT-based robotic vehicle capable of remote control, obstacle detection, voice command navigation, and real-time video streaming.

The rover integrates Arduino Uno, ESP32-CAM, Bluetooth communication, and ultrasonic sensing to create a smart robotic system.

Applications

Security surveillance robots

Disaster monitoring

Military reconnaissance

Educational robotics projects

------------------------------------------

⭐ Features

✅ Bluetooth Controlled Rover

✅ Voice Command Navigation

✅ Real-time Video Streaming (ESP32-CAM)

✅ Obstacle Detection and Avoidance

✅ Servo-based scanning system

✅ Autonomous navigation

✅ Solar powered charging system

------------------------------------------

🧰 Hardware Components

| Component                   | Description               |
| --------------------------- | ------------------------- |
| Arduino Uno R3              | Main microcontroller      |
| ESP32-CAM                   | Wireless video camera     |
| L298N Motor Driver          | Controls DC motors        |
| Ultrasonic Sensor (HC-SR04) | Detects obstacles         |
| Servo Motor                 | Rotates ultrasonic sensor |
| HC-06 Bluetooth Module      | Wireless communication    |
| Solar Panel (6V)            | Power generation          |
| TP4056 Charging Module      | Battery charging module   |
| 18650 Li-ion Battery        | Power supply              |
| LED & Resistors             | Status indicators         |
| Robot Chassis               | Mechanical body           |

------------------------------------------

🛰 System Architecture

Mobile App / Voice Commands
           │
           ▼
      Bluetooth (HC-06)
           │
           ▼
        Arduino Uno
           │
   ┌───────┴────────┐
   ▼                ▼
Motor Driver     Ultrasonic Sensor
  (L298N)            │
   │                 ▼
   ▼             Servo Motor
DC Motors            │
   │                 ▼
 Rover Movement  Obstacle Detection

------------------------------------------

 📷 Camera Streaming Architecture

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

------------------------------------------

🔌 Hardware Connections
  Motor Driver (L298N)

| L298N Pin | Arduino Pin |
| --------- | ----------- |
| ENA       | 10          |
| IN1       | 9           |
| IN2       | 8           |
| IN3       | 7           |
| IN4       | 6           |
| ENB       | 5           |

------------------------------------------

Bluetooth Module (HC-06)

| HC-06 | Arduino |
| ----- | ------- |
| VCC   | 5V      |
| GND   | GND     |
| RX    | Pin 3   |
| TX    | Pin 2   |

------------------------------------------

Ultrasonic Sensor

| Sensor  | Arduino |
| ------- | ------- |
| VCC     | 5V      |
| GND     | GND     |
| Echo    | A2      |
| Trigger | A3      |

------------------------------------------

Servo Motor

| Servo  | Arduino |
| ------ | ------- |
| Signal | A4      |
| VCC    | 5V      |
| GND    | GND     |

------------------------------------------

📷 ESP32-CAM Programming Connections

To upload code to ESP32-CAM, use an FTDI programmer.

| ESP32-CAM | FTDI              |
| --------- | ----------------- |
| 5V        | VCC               |
| GND       | GND               |
| U0R       | TX                |
| U0T       | RX                |
| IO0       | GND (Upload Mode) |


After uploading the code:

Disconnect IO0 from GND

Press RESET

Open browser with ESP32 IP address

Example:
http://192.168.1.100

------------------------------------------

⚙ Installation
Step 1

Install Arduino IDE

Step 2

Upload Arduino rover control code

Step 3

Upload ESP32-CAM streaming code

Step 4

Insert 18650 battery

Step 5

Connect mobile with HC-06 Bluetooth

Step 6

Open camera stream in browser

------------------------------------------

⚡ Working Principle

User sends command through mobile app

Bluetooth module receives command

Arduino processes instructions

Motor driver controls rover movement

Ultrasonic sensor detects obstacles

Servo motor scans environment

Rover avoids obstacles automatically

ESP32-CAM streams video through WiFi

------------------------------------------

👨‍💻 Team Members

| Name                     | Contribution                  |
| ------------------------ | ----------------------------- |
| **D Sree Bhargav Reddy** | Model connections & coding    |
| M Abhiram Reddy          | Model assembly & coding       |
| Arjun Arun               | PPT preparation & connections |
| B Sravan Kumar Reddy     | Documentation                 |
| K Babu                   | Report preparation            |

------------------------------------------

🎓 Institution

Presidency University
School of Computer Science & Engineering
