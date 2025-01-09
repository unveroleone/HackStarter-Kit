# M5Stick Connection Guide

This document provides an overview of the M5Stick's pin layout and the various modules you can connect to it. Whether you're working with wireless modules like the NRF24 or communication devices like the CC1101, this guide will help you set up and wire your components correctly.

---

## 🔍 **Description**

The **M5Stick** is a compact and versatile development board equipped with several GPIO pins, power outputs, and communication protocols. It supports various modules, this makes it really fun.

---

## 🛠 **Pin Legend**

Here is an overview of the M5Stick's pins and their functions:

| **Pin**        | **Description**          | **Voltage**    |
|-----------------|--------------------------|----------------|
| `GND`          | Ground                   | -              |
| `5V`           | 5V Power Supply          | 5V            |
| `3.3V`         | 3.3V Power Supply        | 3.3V          |
| `GPIO26`       | Digital Input/Output     | 3.3V          |
| `GPIO36` (VP)  | Analog Input             | 3.3V          |
| `GPIO0`        | Digital Input/Output     | 3.3V          |

*Note: Always ensure that external modules match the pin voltage requirements.*

---

## 📦 **Compatible Modules**

### 🛰 **1. NRF24 Module**
- **Connections**:
  - `GND` -> GND
  - `VCC` -> 3.3V
  - `CE` -> GPIO26
  - `CSN` -> GPIO0
  - `SCK` -> GPIO18
  - `MOSI` -> GPIO23
  - `MISO` -> GPIO19

- **Wiring Diagram**:
  ![NRF24 Wiring](https://drive.google.com/uc?export=view&id=1xBcZJMhrMP7j8BK8VYRYgAvM96SoFX6b)

*Note: On the picture the module is reversed. The pins have to look down*
---

### 📡 **2. CC1101 RF Module**
- **Connections**:
  - `GND` -> GND
  - `VCC` -> 3.3V
  - `CS` -> GPIO5
  - `SCK` -> GPIO18
  - `MOSI` -> GPIO23
  - `MISO` -> GPIO19

- **Wiring Diagram**:
  ![CC1101 Wiring](https://drive.google.com/uc?export=view&id=19YsKtDgeHgKX49PFT0sgW5vY2RNkxpN_)

*Note: On the picture the module is reversed. The pins have to look down*
---

### **USB Module**
- **Connections**:
  - `GND` -> GND
  - `VCC` -> 3.3V
  - `SDA` -> GPIO21
  - `SCL` -> GPIO22

- **Wiring Diagram**:
  ![USB Wiring](https://drive.google.com/uc?export=view&id=1y0iERMvauCpMxdgUVYGjK9EnBhBoqlyr)

---

### **FM Radio Module**
- **Connections**:
  - `GND` -> GND
  - `VCC` -> 5V
  - `RX` -> GPIO16
  - `TX` -> GPIO17

- **Wiring Diagram**:
  ![FM Wiring](https://drive.google.com/uc?export=view&id=1Wt4f2bYGSTDXmpcBsIoKH_kEIfLFnQAI)

---

### **Micro SD Module**
- **Connections**:
  - `GND` -> GND
  - `VCC` -> 5V
  - `RX` -> GPIO16
  - `TX` -> GPIO17

- **Wiring Diagram**:
  ![SD Wiring](https://drive.google.com/uc?export=view&id=16YZvByd64_GZ9hfrh-mMrGUYC29ud6JG)

---

### **NFC Module**
- **Connections**:
  - `GND` -> GND
  - `VCC` -> 5V
  - `RX` -> GPIO16
  - `TX` -> GPIO17

- **Wiring Diagram**:
  ![NFC Wiring](https://drive.google.com/uc?export=view&id=1pspMFNEtbzl0-3UlL-YOjU5itKGpCsMw)

---

## 📝 **Notes**

1. **Voltage Levels:** Always verify the voltage requirements of the connected modules.
2. **Code Examples:** For each module, refer to the M5Stick documentation or relevant libraries for implementation.
3. **Testing:** Test your connections with a multimeter before powering the M5Stick to prevent damage.

---

## 📚 **Resources**

- [M5Stick Documentation](https://docs.m5stack.com)
- [NRF24 Library](https://github.com/nrf24)
- [CC1101 Guide](https://github.com/cc1101)

