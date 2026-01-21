# Tracking System using LoRa Protocol with STM32

This repository implements a **wireless tracking system** using the **LoRa protocol** and **STM32 microcontrollers**. The system is designed as a **point-to-point communication model**, consisting of a **MASTER node** (GPS transmitter) and a **SLAVE node** (data receiver and display).
![Image](https://github.com/user-attachments/assets/a618e6f6-584b-42c2-801e-b04147943972)

---

## 📌 Project Overview

The project demonstrates how to integrate:
- **LoRa long-range wireless communication**
- **GPS-based location tracking**
- **STM32F103C8T6 (Blue Pill) microcontroller**
- **LCD display via I2C**

### System Architecture

- **MASTER Node**
  - Reads GPS data (latitude & longitude)
  - Transmits tracking data via LoRa

- **SLAVE Node**
  - Receives LoRa packets
  - Displays received GPS coordinates on an LCD

---

## 🚀 Features

- Long-range, low-power LoRa communication
- Real-time GPS tracking
- Simple point-to-point topology
- Modular firmware structure (MASTER / SLAVE)
- STM32 HAL-based implementation

---

## 🛠 Hardware Requirements

| Component | Description |
|---------|-------------|
| STM32F103C8T6 | Main microcontroller |
| LoRa Module (SX1278 / RA-02) | Wireless communication |
| GPS Module (Quectel L80-M39) | Location data |
| 16x2 LCD + I2C module | Display (SLAVE node) |
| 3.3V Power Supply | Stable power source |

---

## 🔌 Pin Configuration (Typical)

### LoRa Module (SPI)

| STM32 | LoRa |
|------|------|
| MOSI | MOSI |
| MISO | MISO |
| SCK  | SCK  |
| GPIO | NSS (CS) |
| GPIO | RESET |
| GPIO | DIO0 |
| 3.3V | VCC |
| GND  | GND |

> ⚠️ Pin mappings may vary depending on your hardware setup.

---

### GPS Module (UART – MASTER Node)

- GPS TX → STM32 RX  
- GPS RX → STM32 TX  
- Power: 3.3V  

---

### LCD Display (I2C – SLAVE Node)

- SDA → STM32 SDA  
- SCL → STM32 SCL  
- Power: 3.3V / 5V (depending on module)

---

## 💻 Software Requirements

- **STM32CubeIDE**
- STM32 HAL Drivers
- LoRa driver/library (e.g. SX1278)
- Basic knowledge of:
  - SPI
  - UART
  - I2C
  - Embedded C

---
## PCB Design
![Image](https://github.com/user-attachments/assets/872c47e4-c8d2-4fa3-ac78-154d065836ed)

---
## ⚙️ Build & Flash

1. Clone the repository:
   ```bash
   git clone https://github.com/namth1793/Tracking-System-using-LoRa-protocol-with-STM32.git

