# 🧠 STM32-Based Smart Embedded Hub

This is a compact, 4-layer embedded board designed to serve as a **core system** in connected products that need precision sensing, motor control, and multiple communication interfaces — all on one board.

---

## 🔧 Key Features

- **STM32F407** microcontroller with onboard debugger (STM32F103)
- **24-bit ADC** (ADS122C04) for high-resolution sensor measurements (0–10 mV differential)
- **2x 36W bi-directional DC motor control** using DRV8701 + MOSFET bridge
- **High-speed communication interfaces:**  
  - Ethernet (2MB/s)  
  - CAN (1MB/s)  
  - USB 2.0  
  - UARTs  
- **Audio support** via stereo DAC (I2C) + microphone codec input
- **Onboard regulation, clocking, and connector support**
- Designed in **Altium Designer** with a **4-layer stack-up**

---

## ⚡ Functions of the Board

This board acts as a **smart embedded brain** that performs the following real-world functions:

### 🎛️ 1. **Sensor Signal Acquisition**
- Measures very small differential analog signals (e.g., from pressure sensors or load cells)
- Converts them to 24-bit digital data using a precision ADC

### 🔌 2. **Communication & Data Transfer**
- Sends and receives data using:
  - **Ethernet** for high-speed network communication
  - **CAN bus** for industrial or automotive interfaces
  - **USB 2.0** for PC connection
  - **UART** for debugging or sensor comms

### ⚙️ 3. **Bi-directional Motor Control**
- Drives **two 36W DC motors** (12V, 3A each)
- Supports speed (PWM) and direction control
- Includes protection using external MOSFET bridges

### 🎤 4. **Audio Input and Output**
- Plays audio to speakers/headphones
- Captures audio from a microphone
- Ideal for alarms, feedback sounds, or voice input

### 🧠 5. **Main System Control**
- Runs embedded firmware to handle all logic, coordination, data routing, and decisions
- Suitable for use in smart devices, robotics, automation, or instrumentation systems

---

## 📐 PCB Snapshots

### 📘 Layout  
<img src="controller-layout.png" width="500" alt="Layout">

### 🧊 3D Top View  
<img src="3D-top-view.png" width="500" alt="3D Top">

### 🔄 3D Bottom View  
<img src="3D-bottom-view.png" width="500" alt="3D Bottom">

---

## ⚙️ Functional Highlights

| Subsystem | Function |
|-----------|----------|
| **Precision ADC** | Reads microvolt-level differential signals (e.g., load cells) |
| **Motor Drivers** | Dual full H-bridge using DRV8701 + external FETs |
| **MCU** | STM32F407 runs core logic + comms |
| **Audio Interface** | Headphone DAC + Mic input via I2C |
| **Interfaces** | Ethernet, CAN, USB, UART |
| **Power** | 12V input, with onboard conversion and protection |

---

## 🧠 What I Learned

- Designing multi-domain systems: analog + power + digital + audio  
- High-speed routing (USB, CAN, Ethernet) on 4-layer stackups  
- Best practices for signal integrity, return paths, and EMI control  
- Isolating noisy power loads from sensitive analog front ends

---

## ⚙️ 📁 Design Tools

- ✅ Schematic + PCB in Altium  
- 📸 PCBWay Trace Width Calculator for PCB width design. 

---


**🔙 [Back to Home](../../README.md)**
