# Smart-Speed-Breaker-Assist-System
IT is an Arduino-based system that uses an HC-SR04 ultrasonic sensor to detect speed breakers ahead. It lowers two DC motors’ speed in zones using PWM via an L298N, then ramps speed back up gradually after crossing. An OLED shows live distance, speed % and zone status.
# 🚗 EMBEDDED SPEED BREAKER DETECTOR
### Smart Vehicle Safety System Using Embedded Technology

<p align="center">
  <strong>An intelligent embedded system designed to detect road speed breakers and alert drivers using sensor-based monitoring.</strong>
</p>

---

## 📌 Project Overview

The **Embedded Speed Breaker Detector** is a smart vehicle safety system designed to identify speed breakers and sudden road irregularities using an accelerometer-based detection mechanism.

The system uses an ESP32 microcontroller and an MPU6050 accelerometer and gyroscope sensor to continuously monitor vehicle movement and detect sudden vertical acceleration changes caused by speed breakers.

With GPS integration, the system can record the geographical locations of detected speed breakers. A buzzer and display provide alerts to improve driver awareness and promote safer driving.

The proposed system aims to reduce unexpected vehicle impacts, improve road awareness, and support intelligent transportation systems.

## 🎯 Objectives

- Detect speed breakers using real-time acceleration data.
- Monitor vehicle vibrations and sudden movements.
- Identify and record speed breaker locations using GPS.
- Provide immediate alerts through a buzzer and display.
- Develop a low-cost and efficient embedded safety solution.
- Explore future integration with IoT-based road monitoring systems.

## ⚙️ Key Features

- **Real-Time Detection:** Continuously monitors vehicle acceleration and movement.
- **Vibration Analysis:** Identifies sudden changes in acceleration.
- **GPS Location Tracking:** Records the geographical coordinates of detected road obstacles.
- **Driver Alert System:** Provides buzzer and visual notifications.
- **Embedded Processing:** Performs sensor data processing using ESP32.
- **Expandable Architecture:** Supports future IoT and cloud integration.

## 🧰 Hardware Requirements

| Component | Function |
|---|---|
| ESP32 Development Board | Main microcontroller |
| MPU6050 | Accelerometer and gyroscope |
| NEO-6M GPS Module | Location tracking |
| OLED Display | Information display |
| Buzzer | Audio alert |
| LED | Visual indication |
| Jumper Wires | Circuit connections |
| Power Supply | System power |

## 💻 Software Requirements

- Arduino IDE
- Embedded C / Arduino C++
- ESP32 Board Package
- Adafruit MPU6050 Library
- Adafruit Unified Sensor Library
- TinyGPS++ Library
- Wire Library

## 🔌 System Architecture

```text
       MPU6050 SENSOR
              |
              v
       ESP32 MICROCONTROLLER
              |
       +------+------+
       |      |      |
       v      v      v
      GPS   BUZZER  OLED
       |      |      |
       v      v      v
    LOCATION ALERT DISPLAY
       |
       v
  SPEED BREAKER DATA
```

## 🔄 Working Principle

1. The MPU6050 continuously measures acceleration and angular velocity.
2. The ESP32 receives and processes sensor readings.
3. The system analyzes vertical acceleration changes to identify possible speed breakers.
4. When the measured acceleration crosses a calibrated detection threshold, the system identifies a possible road bump.
5. The GPS module obtains the current geographical coordinates.
6. The buzzer and display notify the driver.
7. The detected event and location can be recorded for future reference.

## 📂 Project Structure

```text
Embedded-Speed-Breaker-Detector/
│
├── src/
│   └── main.ino
│
├── docs/
│   ├── circuit-diagram.png
│   └── system-architecture.png
│
├── images/
│   └── project-prototype.png
│
├── README.md
├── LICENSE
└── .gitignore
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Embedded-Speed-Breaker-Detector.git
```

### 2. Open the Project

Open the `main.ino` file using Arduino IDE.

### 3. Install Required Libraries

Install the required libraries through Arduino IDE Library Manager.

### 4. Configure ESP32

- Select your ESP32 development board.
- Select the appropriate COM port.
- Configure the sensor and GPS pins according to the circuit diagram.

### 5. Upload the Code

Connect the ESP32 to your computer and upload the firmware.

### 6. Test the System

Move the sensor carefully to simulate road vibrations and verify the detection and alert mechanism.

## 📊 Applications

- Smart vehicle safety systems
- Intelligent transportation systems
- Road condition monitoring
- Automotive embedded systems
- Smart city infrastructure
- Road hazard mapping

## 🔮 Future Enhancements

- IoT-based speed breaker location sharing.
- Mobile application integration.
- Cloud-based road condition monitoring.
- Community-based speed breaker mapping.
- Machine learning-based road anomaly classification.
- Integration with vehicle navigation systems.
- Driver notification before reaching a previously detected speed breaker.

## ⚠️ Limitations

- Detection accuracy depends on sensor calibration and vehicle suspension.
- GPS accuracy may vary depending on environmental conditions.
- Different road surfaces can produce similar acceleration patterns.
- The prototype requires real-vehicle testing before practical deployment.
- This project is an experimental driver-assistance prototype, not a certified automotive safety device.

## 👨‍💻 Developer

**Nithish Kumar R**

Electronics and Communication Engineering

KPR Institute of Engineering and Technology

**Project:** Embedded Speed Breaker Detector – Smart Vehicle Safety System

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

<p align="center">
  <strong>Built with ❤️ using Embedded Systems and IoT Technology</strong>
</p>
