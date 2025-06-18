# 🗑️ Smart Dustbin Automation (Arduino)

An automated smart dustbin that opens its lid when a user is nearby and alerts when the bin is nearly full using ultrasonic sensors, a servo motor, and a buzzer.

## 📷 Features

- **Auto Lid Opening**: Opens when a hand/object is detected within 15 cm.
- **Auto Lid Closing**: Closes after 3 seconds.
- **Fullness Detection**: Buzzer alert when trash level is near the top (15 cm or less).
- **Serial Monitor Output**: Debugging information printed to serial monitor.

## 🧰 Hardware Requirements

- Arduino UNO
- 2 × HC-SR04 Ultrasonic Sensors
- SG90 Servo Motor
- Buzzer
- Breadboard and Jumper Wires
- USB Cable

## ⚡ Circuit Connections

| Component       | Arduino Pin |
|----------------|-------------|
| TRIG_TOP       | 9           |
| ECHO_TOP       | 8           |
| TRIG_BOT       | 5           |
| ECHO_BOT       | 4           |
| Servo Signal   | 3           |
| Buzzer (+)     | 10          |

## 🚀 Getting Started

1. Open `SmartDustbin.ino` in the Arduino IDE.
2. Connect your Arduino via USB.
3. Upload the code.
4. Open Serial Monitor to observe distance readings.

## 🧠 How It Works

- **Top Sensor**: Detects if a hand/object is near the lid. If within 15 cm, opens the lid using the servo.
- **Bottom Sensor**: Measures trash level. If trash comes within 15 cm of the sensor, the buzzer alerts the user.
- **Servo**: Moves lid to 90° when triggered, and back to 0° after 3 seconds.

## 📸 Demo

*(Add a photo or video GIF of the working prototype here)*

---

> Created by [Shreyash Shrishette]  
