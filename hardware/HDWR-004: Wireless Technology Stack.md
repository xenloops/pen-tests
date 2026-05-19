# Wireless Technology Stack

CWE-319

Risks: Authentication, Authorization, Component Vulnerabilities, Information Exposure 

## Description

Wireless technologies including WiFi, Bluetooth Low Energy (BLE), and Zigbee can be used to transmit data for a variety of applications and network topologies. Wireless networks can be susceptible to vulnerabilities both in design and execution. 

## Tools

* Manual
* Kali Tools(Air-crackng, Reaver, etc)
* btlejack (Microbit)
* Attify Apimote. 

## Test

Test the wireless network technology implemented on the device for MITM, DoS, Evil Twin, and other attacks where Availability, Integrity, and/or Confidentiality are compromised. Critical information can be either stolen or spoofed. The networking technology stack used must also be resistant to similar attacks.

## Results

The test constitutes a failure if unauthorized access to the wireless technology results in any change to the transmission, reception or storage of data on the device or participating clients. 

## Impact
