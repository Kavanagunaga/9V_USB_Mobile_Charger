
# 9V USB Mobile Charger

A regulated 9V DC mobile charger designed and implemented using a step-down transformer, bridge rectifier, filter capacitor, and 7809 voltage regulator. The project was simulated in Proteus and implemented on hardware using a perfboard.

## 📌 Project Overview

The 9V USB Mobile Charger converts 230V AC mains supply into a regulated 9V DC output suitable for powering/charging compatible USB devices.

The system consists of:

- Step-down transformer
- Bridge rectifier using 1N4007 diodes
- Filter capacitor
- 7809 voltage regulator
- Fuse for protection
- USB connector
- Heat sink for the regulator

The circuit was first verified through simulation and then implemented on hardware. The final output was measured to be approximately 9V DC, and the prototype was successfully used to charge a mobile phone during testing. 

## 🎯 Objectives

- Design a safe AC-to-DC power supply.
- Convert 230V AC into a regulated 9V DC output.
- Use a 7809 voltage regulator for voltage regulation.
- Obtain a stable output under load.
- Verify the circuit through Proteus simulation.
- Implement and test the circuit on hardware.
- Provide fuse protection against excessive current.

## ⚙️ System Architecture

```text
       230V AC
          │
          ▼
 ┌─────────────────┐
 │ Step-Down       │
 │ Transformer     │
 │ 230V → 12V AC   │
 └─────────────────┘
          │
          ▼
 ┌─────────────────┐
 │ Bridge          │
 │ Rectifier       │
 │ 4 × 1N4007      │
 └─────────────────┘
          │
          ▼
 ┌─────────────────┐
 │ Filter          │
 │ Capacitor       │
 │ 1000µF          │
 └─────────────────┘
          │
          ▼
 ┌─────────────────┐
 │ 7809 Voltage    │
 │ Regulator       │
 └─────────────────┘
          │
          ▼
      Fuse
          │
          ▼
     9V DC Output
          │
          ▼
    USB Connector
