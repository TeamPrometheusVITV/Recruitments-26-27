![Team Banner](/images/Team%20Banner.png)

# ⚡ Team Prometheus — Electrical Recruitment Task 2026–27

Welcome to the _Electrical Team Recruitment 2026–27_ for _Team Prometheus_.  
This repository contains _two tasks_ designed to evaluate your understanding of electrical engineering concepts, circuit design, and hardware integration in the context of _robotic soccer_.

---

## 🧩 Task 1: Balance and Motion Control System

### 🔍 Overview

In this task, you will:

- _Design a Balance Control Prototype_ in TinkerCAD

  - Use an _MPU6050_ to detect tilt and orientation.
  - Interface the sensor with an _Arduino_ or _ESP32_ microcontroller.
  - Use _servo motors_ to simulate real-time balancing correction.

- _Implement Feedback & Safety Indicators_
  - Use _LEDs_ or a _buzzer_ to indicate loss of balance or error states.
  - Display real-time sensor readings (angles or acceleration) on the _Serial Monitor_.

### 💡 Clarification

A _Balance and Motion Control System_ is crucial in humanoid robots to help them remain upright and recover from disturbances — similar to how humans adjust their body posture.

### 📦 Deliverables

- A _TinkerCAD_ simulation showing active balance correction using feedback control.
- _Arduino implementation_ of sensor-based motion correction.
- A _report_ including:
  - Component justification (e.g., why MPU6050, why servos, etc.)
  - Control logic explanation (how tilt translates to motor correction)
  - Relevance of the system in humanoid soccer applications

---

## 🔋 Task 2: Power and Sensor Management PCB

### 🔍 Overview

In this task, you will:

- _Design a Single-Layer PCB_ for Power Distribution and Sensor Integration
  - Include a _microcontroller (ESP32)_
  - Add ports for _sensors_ (MPU6050, ultrasonic, temperature) and _servo outputs_
  - Implement _voltage regulation (LM7805)_
  - Use _diagnostic LEDs_ to indicate power and signal status.

### 🎯 Focus Areas

- Clean and compact routing suitable for a humanoid robot’s constrained structure.
- Stable power delivery and minimal electrical noise.
- Expandability for future sensor or actuator modules.

### 💡 Clarification

Your PCB should act as a _central hub_ connecting the robot’s sensors, actuators, and control unit — think of it as the _“nervous system”_ of your humanoid robot.

### 📦 Deliverables

- _Schematic and PCB layout_ (KiCad, Eagle, or Altium).
- [Optional] _Gerber files_ ready for fabrication.
- A _report_ detailing:
  - Design reasoning and component selection.
  - PCB layout strategy (trace routing, decoupling, ground plane usage).
  - Challenges faced and how they were resolved.

---

## 📘 Summary

| Task     | Description                   | Tools                    | Key Deliverables               |
| -------- | ----------------------------- | ------------------------ | ------------------------------ |
| _Task 1_ | Balance and Motion Control    | TinkerCAD, Arduino/ESP32 | Simulation, Code, Report       |
| _Task 2_ | Power & Sensor Management PCB | KiCad/Eagle/Altium       | Schematic, PCB, Gerber, Report |

---

### 🧠 Note

> Ensure all your files are _clearly named, your **simulation links are accessible, and your **report is concise yet descriptive_.

---

_Team Prometheus — Electrical Recruitment Task 2026–27_
