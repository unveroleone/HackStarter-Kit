# M5Stick Connection Guide

This document provides an overview of the M5Stick's pin layout and the various modules you can connect to it. Whether you're working with wireless modules like the NRF24 or communication devices like the CC1101, this guide will help you set up and wire your components correctly.

---

## 🔍 **Description**

The **M5Stick** is a compact and versatile development board equipped with several GPIO pins, power outputs, and communication protocols. It supports various modules, making it perfect for IoT projects.

---

## 📝 **Notes**

1. **Information:** If you don't know how a module works or where to buy it, check the [MyProducts](../../MyProducts/README.md) page.
2. **Attention:** Some modules in the pictures are shown upside down. This means the pins on the module may need to face down in most cases.
3. **How to use:** If you're unsure where or how to use the modules, or need additional tools, visit the [HackingTheory](../HackingTheory/README.md) page.

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

### **1. NRF24 Module**
- **Connections:**
  - `GND` -> GND
  - `VCC` -> 3.3V
  - `CE` -> GPIO26
  - `CSN` -> GPIO33
  - `SCK` -> GPIO18
  - `MOSI` -> GPIO23
  - `MISO` -> GPIO19


  <img src="https://drive.google.com/uc?export=view&id=1xBcZJMhrMP7j8BK8VYRYgAvM96SoFX6b" alt="NRF24 Wiring" style="width: 50%; height: auto;">

---

### **2. CC1101 RF Module**
- **Connections:**
  - `GND` -> GND
  - `VCC` -> 3.3V
  - `CS` -> GPIO33
  - `SCK` -> GPIO18
  - `MOSI` -> GPIO23
  - `MISO` -> GPIO19


  <img src="https://drive.google.com/uc?export=view&id=19YsKtDgeHgKX49PFT0sgW5vY2RNkxpN_" alt="CC1101 Wiring" style="width: 50%; height: auto;">

---

### **3. USB Module**
- **Connections:**
  - `GND` -> GND
  - `VCC` -> 5V
  - `D+` -> GPIO32
  - `D-` -> GPIO33


  <img src="https://drive.google.com/uc?export=view&id=1y0iERMvauCpMxdgUVYGjK9EnBhBoqlyr" alt="USB Wiring" style="width: 50%; height: auto;">

---

### **4. FM Radio Module**
- **Connections:**
  - `GND` -> GND
  - `VCC` -> 3.3V
  - `SDA` -> GPIO21
  - `SCL` -> GPIO22


  <img src="https://drive.google.com/uc?export=view&id=1Wt4f2bYGSTDXmpcBsIoKH_kEIfLFnQAI" alt="FM Radio Wiring" style="width: 50%; height: auto;">

---

### **5. Micro SD Module**
- **Connections:**
  - `GND` -> GND
  - `VCC` -> 3.3V
  - `CS` -> GPIO33
  - `CLK` -> GPIO18
  - `MOSI` -> GPIO23
  - `MISO` -> GPIO19


  <img src="https://drive.google.com/uc?export=view&id=16YZvByd64_GZ9hfrh-mMrGUYC29ud6JG" alt="Micro SD Wiring" style="width: 50%; height: auto;">

---

### **6. NFC Module**
- **Connections:**
  - `GND` -> GND
  - `VCC` -> 3.3V
  - `SDA` -> GPIO21
  - `SCL` -> GPIO22


  <img src="https://drive.google.com/uc?export=view&id=1pspMFNEtbzl0-3UlL-YOjU5itKGpCsMw" alt="NFC Module Wiring" style="width: 50%; height: auto;">

---

If you have any ideas or feedback, feel free to contact me!
