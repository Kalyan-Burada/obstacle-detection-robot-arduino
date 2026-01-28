# Obstacle Detection Robot using Arduino

An autonomous obstacle detection robot developed using an **Arduino Uno** and **ultrasonic sensor**, capable of navigating its environment by detecting and avoiding obstacles in real time without human intervention.

---

## 📌 Project Overview

Robotics plays a crucial role in modern automation across sectors such as **manufacturing, healthcare, military, construction, and autonomous vehicles**.  
This project focuses on designing and implementing an **automatic obstacle detection robot** that senses nearby objects and intelligently changes its direction to avoid collisions.

Inspired by real-world technologies such as **self-driving cars**, the robot continuously monitors its surroundings and makes movement decisions dynamically.

---

## 🎯 Objectives

- Design an autonomous mobile robot
- Detect obstacles using an ultrasonic distance sensor
- Avoid collisions by changing direction intelligently
- Implement real-time decision-making using Arduino
- Demonstrate applications of embedded systems and robotics

---

## 🧠 Working Principle

1. The ultrasonic sensor emits sound waves and measures the echo time.
2. Distance to obstacles is calculated using the echo response.
3. If an obstacle is detected within a threshold distance:
   - The robot stops
   - Scans left and right using a servo-mounted sensor
   - Chooses the direction with maximum free space
4. If no obstacle is detected, the robot continues moving forward.

This logic enables **autonomous navigation in dynamic environments**.

---

## 🛠️ Components Used

- **Arduino Uno Microcontroller**
- **Ultrasonic Sensor (HC-SR04)**
- **L298N Motor Driver**
- **DC Motors with Wheels**
- **Servo Motor**
- **Chassis**
- **Battery**
- **Connecting Wires**

---

## 🔌 Circuit Diagram

The circuit consists of:
- Arduino Uno connected to the ultrasonic sensor (Trig & Echo pins)
- L298N motor driver controlling two DC motors
- Servo motor mounted with ultrasonic sensor for directional scanning

📁 Circuit diagram is available in the `circuit-diagram/` folder.

---

## 📚 Libraries Used

```cpp
#include <Servo.h>
#include <NewPing.h>
