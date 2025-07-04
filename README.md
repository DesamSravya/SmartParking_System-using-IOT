# 🚗 Automated Car Parking System using Arduino

This project demonstrates a simple and effective **Automated Car Parking System** using Arduino. It uses IR sensors to detect vehicle entry and exit, a servo motor to control the parking gate, and keeps track of available parking slots.

## 📦 Features

- Detects car entry and exit using IR sensors
- Automatically opens and closes the gate using a servo motor
- Displays available parking slots in the Serial Monitor
- Prevents entry when slots are full
- Compact and beginner-friendly implementation

## 🛠️ Components Used

- Arduino Uno
- 2x IR Sensors
- 1x Servo Motor
- Jumper Wires
- USB Cable
- Breadboard

## 🔌 Circuit Overview

- **IR Sensor 1**: Detects vehicle at the entry
- **IR Sensor 2**: Detects vehicle at the gate/exit
- **Servo Motor**: Controls the parking gate barrier
- **Arduino Pins**:
  - IR1: Pin 2
  - IR2: Pin 4
  - Servo: Pin 3

## 🧠 Logic

1. If a vehicle is detected by IR1 and slots are available:
   - Gate opens
   - Car passes IR2
   - Gate closes
   - Slot count decreases
2. If all slots are full:
   - Displays "SORRY..!! Parking Full"
3. If a car exits (detected by IR2):
   - Slot count increases

## 📟 Output

Check the Serial Monitor at 9600 baud rate for updates:
