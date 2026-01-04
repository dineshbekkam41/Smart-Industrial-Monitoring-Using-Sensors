

# 🔌 Smart IoT-Based Multi-Sensor Monitoring System (Arduino)

## 📌 Project Overview

This project is a **Smart IoT-based Multi-Sensor Monitoring System** developed using **Arduino UNO** and executed using the **Arduino IDE**.
It integrates multiple sensors to **monitor environmental conditions and respond automatically** using actuators like a buzzer, LED, and motor (fan).

The system continuously monitors:

* Gas leakage
* Temperature
* Light intensity
* Distance (obstacle detection)

Based on sensor readings, it triggers alerts and control actions in real time.

---

## 🎯 Objectives

* Detect **gas leakage** and alert users
* Monitor **temperature** and control a cooling fan
* Automatically control **lighting** based on light intensity
* Measure **distance** using ultrasonic sensing
* Display real-time sensor data via **Serial Monitor**

---

## 🧰 Components Used

* Arduino UNO
* MQ-2 Gas Sensor
* LM35 Temperature Sensor
* LDR (Light Dependent Resistor)
* Ultrasonic Sensor (HC-SR04)
* Buzzer
* DC Motor / Fan
* LEDs
* Breadboard
* Jumper Wires
* USB Cable

---

## ⚙️ System Functionality

### 🔥 Gas Detection (MQ-2)

* Reads gas concentration via analog pin
* If gas level exceeds a predefined threshold:

  * **Buzzer ON**
  * **Warning LED ON**

### 🌡️ Temperature Monitoring (LM35)

* Continuously measures temperature
* If temperature > **38°C**:

  * **Fan (Motor) turns ON**
* Else:

  * Fan remains OFF

### 💡 Light Detection (LDR)

* Detects ambient light intensity
* If environment is dark:

  * **LED turns ON**
* Else:

  * LED turns OFF

### 📏 Distance Measurement (Ultrasonic Sensor)

* Calculates distance using echo time
* Distance displayed on Serial Monitor in **centimeters**

---

## 🔌 Pin Configuration

| Component               | Arduino Pin |
| ----------------------- | ----------- |
| MQ-2 Gas Sensor         | A0          |
| Buzzer                  | D8          |
| Gas LED                 | D0          |
| LM35 Temperature Sensor | A5          |
| Motor (Fan)             | D5          |
| LDR                     | A0          |
| LDR LED                 | D7          |
| Ultrasonic Trigger      | D12         |
| Ultrasonic Echo         | D11         |

---

## 🧠 Logic & Thresholds

* Gas Threshold: **400**
* Temperature Threshold: **38°C**
* LDR Dark Condition: **< 150**
* Data refresh delay: **5 seconds**

---

## 🖥️ Software Requirements

* **Arduino IDE**
* USB Driver for Arduino UNO

---


## 📊 Output

* Real-time sensor values displayed on Serial Monitor
* Automatic actuation of:

  * Buzzer
  * LEDs
  * Fan (Motor)

---

## 📸 Project Images

Refer to the project images uploaded in this repository to understand:

* Hardware connections
* Sensor placements
* Overall system layout

---

## 🚀 Applications

* Smart Home Safety Systems
* Industrial Gas Leakage Detection
* Automated Environmental Monitoring
* IoT-based Security Systems
* Academic Mini / Major Projects

---

## 🧑‍💻 Developed Using

* **Arduino Programming (Embedded C)**
* **Arduino IDE**
* **Basic IoT & Sensor Integration Concepts**

---

## 📄 License

This project is for **educational purposes**.
Feel free to modify and enhance it.

---


