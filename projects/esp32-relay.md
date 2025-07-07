# 🔌 ESP32 Relay Control Board

A compact, mains-powered relay interface driven by an ESP32 DevKitC for Wi-Fi/Bluetooth-enabled switching of AC loads.

<img src="../assets/esp32-relay-schematic.png" alt="ESP32 Relay Control Schematic" width="600">

---

## 📋 Overview

This board lets an ESP32 toggle a 5 V relay to control AC line appliances.  
It includes:
- An HLK‑PM05 AC‑DC power module
- A transistor switch (2N2219) with flyback diode
- A 5 V relay and screw terminals for line output
- A layout focused on safety and modularity

---

## 🔩 Components Used
- **MCU:** ESP32 DevKitC
- **Driver Circuit:** 2N2219 NPN + 1N4007
- **Relay:** 5V SPDT
- **Power Module:** HLK‑PM05 (AC‑to‑5V)
- **Design Tool:** KiCad

---

## 💡 Design Considerations

### ✅ Safety
- AC side is completely isolated from logic.
- HLK‑PM05 used for compact, safe power conversion.

### ✅ Protection
- Flyback diode prevents relay coil from damaging the transistor.
- Transistor acts as a current buffer between ESP32 and relay.

### ✅ Modularity
- Screw terminals allow external connections and sensor expansion.
- Clear silkscreen labeling for RELAY_COM, NO, NC, V‑L, and V‑N.

---

## 🧠 What I Learned
- Interfacing low-voltage MCUs with high-voltage relays
- Using certified AC-DC modules safely in mixed-signal PCB design
- Writing ESP32 firmware to toggle relays reliably via GPIO

---

## 🖼️ Images

<img src="../assets/esp32-relay-schematic.png" width="400" alt="Schematic">  
<img src="../assets/esp32-relay-layout.png" width="400" alt="PCB Layout">

---

**Back to [Home](../README.md)**
