# 🔌 ESP32 Relay Control Board

A compact relay board controlled by an ESP32, for switching AC loads safely.

---

## 📋 What it Does
- Lets ESP32 switch a 5V relay to turn ON/OFF AC devices
- Uses a 2N2219 transistor to drive the relay
- Powered by HLK-PM05 (AC to 5V converter)
- Has screw terminals for easy wiring

---

## 🔩 Main Components
- **Microcontroller:** ESP32 DevKitC  
- **Relay:** 5V SPDT  
- **Transistor Driver:** 2N2219 + 1N4007 diode  
- **AC-DC Supply:** HLK-PM05  
- **Software:** Arduino / ESP-IDF

---

## 🧠 What I Learned
- How to safely control AC with low voltage signals
- Transistor switching and flyback protection
- PCB layout for AC + logic separation

---

## 🖼️ Images  

<img src="esp32-relay-schematic.png" width="400">  
<img src="esp32-relay-layout.png" width="400">

---

**🔙 [Back to Home](../../README.md)**
