# Theory Page

This page explains various concepts and techniques related to wireless technologies like WiFi, BLE, and RF, as well as specific modules such as the [NRF24](../../MyProducts/README.md#nrf24-module) or [CC1101](../../MyProducts/README.md#cc1101-module). If you have other topics you’d like me to add, feel free to let me know!

---

## WiFi

For WiFi-related experiments or projects, you will need an ESP32 board.

### Target Attacks

- **How it works:** Devices in a WiFi network communicate through an Access Point (AP). The attacker sends fake deauthentication frames to the client (e.g., a smartphone), mimicking the AP. This disrupts the connection between the client and the AP. This is also known as a **Deauthentication Attack**.
- **Uses:** 
  - Disrupting access to a network.
  - Forcing the victim to connect to a rogue access point.
- **Limitations:** 
  - Only effective in unsecured or poorly configured networks.
  - Works only on 2.4 GHz networks.

### Beacon Spam

- **Description:** Sending fake beacon frames to create fake networks.  
- **Purpose:** Overloading device network lists or distracting users.  
- **Practical Use:** Not practical but often used for fun, like creating fake networks with humorous names.

### Deauth Flood

- **Description:** Flooding the entire 2.4 GHz network with deauthentication frames to disconnect devices.  
- **Usage:** Forcing disconnections, preparing MitM attacks.  
- **Practical Use:** Not practical and primarily used to annoy people.

### Evil Portal

Evil Portals can be highly dangerous, as they involve creating a fake network where users are tricked into logging into a counterfeit page, such as a fake Google login. This allows attackers to steal credentials.  

- **Description:** Setting up a rogue access point with a fake captive portal designed to mimic legitimate websites.  
- **Purpose:** Harvesting user credentials or redirecting victims to malicious sites for further exploitation.  

---

## BLE (Bluetooth Low Energy)

### Media Commands

Media Commands allow you to control a connected device remotely. Once connected, you can perform actions like taking screenshots or adjusting the volume (e.g., increasing or decreasing it).  

- **Description:** Sending commands to manage media playback or system functions on connected BLE devices.  
- **Examples:** Playing, pausing, skipping tracks, taking screenshots, or controlling volume.

### BadBLE

BadBLE takes Media Commands to the next level. It allows you to execute scripts on the connected device. While some scripts are harmless, others can be highly dangerous and potentially critical to the device's functionality or security.  

- **Description:** Executing scripts on connected BLE devices to manipulate their behavior.  
- **Examples:** Running benign tasks or deploying harmful scripts that can disrupt or exploit the target device.  

### BLE Spam

- **Description:** Overwhelming BLE devices with continuous pairing or connection attempts.  
- **Purpose:** Distracting or disabling devices.  
- **Restrictions:** Most devices have security measures in place to prevent such spamming, which can significantly slow down or block the attack.

---

## RF (Radio Frequency)

### Scan and Copy

- **Description:** Scanning RF signals and copying their patterns for later use.  
- **Example:** Copying signals from a garage remote to open it with your device.  
- **Tools:** Modules like the [CC1101](../../MyProducts/README.md#cc1101-module).

### Custom Sub-GHz

- **Description:** Allows the emulation of captured signals or the use of downloaded signal files to perform specific actions.  
- **Example:** Downloading a signal file to open a specific garage door and then executing the action.  
- **Tools:** [CC1101](../../MyProducts/README.md#cc1101-module) module.

### Jammer Full

- **Description:** Transmitting noise signals to disrupt communication on specific RF frequencies.  
- **Purpose:** Disabling remote devices or creating interference.  
- **Practical Use:** Must comply with legal regulations in your country.

---

## NRF24 Jammer (2.4 GHz)

The [NRF24](../../MyProducts/README.md#nrf24-module) module can jam the 2.4 GHz frequency band, affecting protocols like WiFi, BLE, and Zigbee.  

- **Example Use Cases:**  
  - Disrupting WiFi connections.  
  - Preventing BLE devices from pairing or working.  
  - Interfering with Zigbee networks.  
- **Tools and Implementation:** Requires an [NRF24](../../MyProducts/README.md#nrf24-module) module.

---

## Wardriving

I don’t have personal experience with wardriving, but I can explain how it works:

- **Description:** Wardriving involves driving around with specialized equipment to detect and map WiFi networks in a specific area. This can include collecting information like SSIDs, signal strength, and security settings.  
- **Purpose:** Typically used for security assessments but can also be misused to identify vulnerable networks.  
- **Equipment:** A device with WiFi capabilities (e.g., a laptop, smartphone, or microcontroller such as an [M5](../../MyProducts/README.md#M5StickC-PLUS2)) and software for network scanning. GPS integration is often included to map the locations.  

---

## BadUSB

[BadUSB](../../MyProducts/README.md#ch9329-usb-module) works similarly to BadBLE, but instead of being wirelessly connected, you need to physically plug in the device (e.g., an [M5Stack](../../MyProducts/README.md#M5StickC-PLUS2) or similar) to the target system.

- **Description:** Executes preprogrammed scripts or commands once the device is plugged into a system, often mimicking a USB keyboard or other HID device.  
- **Examples:** Automating tasks, injecting malicious scripts, or opening specific applications on the target system.  
- **Limitations:** Requires physical access to the target device.  

---

## Disclaimer

All techniques described here are intended for educational purposes only. Unauthorized use of these methods in real-world scenarios may violate laws and regulations.
