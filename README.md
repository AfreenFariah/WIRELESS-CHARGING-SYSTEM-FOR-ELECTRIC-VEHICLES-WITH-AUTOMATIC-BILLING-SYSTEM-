# Wireless Charging System for Electric Vehicle Batteries with Automatic Billing

## Overview
This project implements a wireless charging system for electric vehicles (EVs) using **Inductively Coupled Power Transfer (ICPT)**. It features automatic vehicle detection and billing using an Arduino microcontroller and current sensor. The system enables safe, efficient, and hands-free charging, with live tracking of consumed power and billing amount on an LCD display.

---

## Features
- Wireless charging via resonant inductive coupling
- IR-based vehicle detection
- Real-time billing calculation
- LCD display for live status and cost
- Microcontroller-controlled switching system

---

## Requirements

### Hardware
- Arduino (CH340)
- KA3525 PWM Controller
- MOSFETs (IRF840)
- IR Sensor
- 24V Relay
- Transformer (12-0-12V / 1A)
- 7809 Voltage Regulator
- TX and RX Coils (LC Resonant Circuit)
- LCD Display (16x2)
- Current Sensor
- Diodes: 1N4007, 1N4148
- Capacitors, Resistors
- LED bulbs, DC Motor

### Software
- Arduino IDE
- Embedded C (Optional: Keil µVision5)
- Serial Monitor (for debugging)

---

## Methodology
1. AC power is converted to regulated DC using transformer, rectifier, and voltage regulator.
2. KA3525 PWM controller generates high-frequency pulses for wireless power transfer.
3. MOSFETs drive the TX coil, creating a magnetic field.
4. RX coil receives the field, converts AC to DC, and charges the EV battery.
5. IR sensor detects vehicle presence and triggers charging.
6. Arduino calculates power usage and cost, displaying it on an LCD.

---

## Working
- Vehicle parks on the platform.
- IR sensor detects the vehicle and activates the TX coil.
- Wireless power is transmitted to the RX coil.
- Power is rectified and used to charge the battery.
- Current sensor tracks energy used.
- Arduino computes and displays billing info on LCD.

---

## Usage
1. Power ON the system.
2. Park EV on the charging platform.
3. IR sensor activates the system and charging begins.
4. Real-time billing and units are displayed on LCD.
5. Charging stops automatically on removal.


---

## College
**Government College of Engineering, Dharmapuri**  
**Department of Electrical and Electronics Engineering**

---

## License
For academic use only. All rights reserved.


