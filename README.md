# Bluetooth-Based Proximity Authentication System


## Project description

The goal is to create and program a small portable device that communicates with a laptop using Bluetooth Low Energy (BLE).

The device or it's driver detects proximity between itself and the laptop. When the device is within approximately **1metre**, the laptop automatically unlocks. When the device moves beyond this distance, the laptop automatically locks.

It should contain a green led
- pulsing indicates that the two device sees eachother
- continues light indicates that it unlocked the laptop

And a button
- push switches it on and off
- holding it for 5 sec starts pairing

## Hardware requirements

- ESP32-S3 microcontroller (ESP32 C3 Super Mini)

- Bluetooth Low Energy communication

- Rechargeable battery

- Battery charging module

- LED indicator

- Push button

- Protective enclosure (optional)

## Software Requirements

- ESP32 firmware (ESP-IDF)

- Bluetooth Low Energy communication (with GATT data protocol)

- Python / c / bash application running on Ubuntu

- RSSI-based proximity estimation

- Cryptographic device authentication

- Ubuntu session locking and unlocking integration

## System Operation

1. The ESP32 device periodically advertises its presence over Bluetooth.

2. The Ubuntu application detects the device and measures its signal strength.

3. The application estimates whether the device is within the configured distance.

4. The device's identity is verified using cryptographic authentication.

5. If the authenticated device is nearby, Ubuntu unlocks the laptop.

6. If the device moves away, Ubuntu automatically locks the session.

## Main Objectives

- Assemble a portable Bluetooth device.

- Implement wireless communication between the device and Ubuntu.

- Estimate physical proximity using Bluetooth signal strength.

- Implement secure device authentication.

- Integrate automatic locking and unlocking into Ubuntu.

- Evaluate the reliability of proximity detection.