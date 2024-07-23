# WT32-ETH01 v1.4 unofficial getting-started

This repository is a collection of challenges solved using the WT32-ETH01 v1.4 and examples of how to use this ESP32-based device in conjunction with the Arduino Core for ESP32.

## Overview

We can describe this as an unofficial getting-started documentation. Due to the lack of concrete examples and easy-to-find answers in the official Wireless Tag documentation, I decided to share what I have discovered.

## Table of Contents

1. [Introduction](#introduction)
2. [Hardware Overview](#hardware-overview)
3. [Getting Started](#getting-started)
    - [Setting Up the Development Environment](#setting-up-the-development-environment)
    - [Basic Connectivity](#basic-connectivity)
4. [Example Projects](#example-projects)
    - [Project 1: Basic Network Setup](#project-1-basic-network-setup)
    - [Project 2: Sensor Integration](#project-2-sensor-integration)
    - [Project 3: Data Logging](#project-3-data-logging)
5. [Troubleshooting](#troubleshooting)
6. [Additional Resources](#additional-resources)
7. [Contributing](#contributing)

## Introduction

The WT32-ETH01 is a versatile module designed by Wireless Tag, based on the popular ESP32 chip, and equipped with an Ethernet interface. This makes it suitable for a wide range of IoT applications that require reliable and wired network connections.

## Hardware Overview

The WT32-ETH01 features:
- ESP32-WROVER-B module
- Ethernet PHY (LAN8720)
- RJ45 connector
- GPIOs for various peripherals

## Getting Started

### Setting Up the Development Environment

To begin working with the WT32-ETH01, you will need:
- A development board (WT32-ETH01 v1.4)
- Arduino IDE or PlatformIO
- USB to TTL adapter for programming
- Ethernet cable and network access

1. **Install the Arduino Core for ESP32:**
   Follow the instructions from the [official ESP32 Arduino GitHub repository](https://github.com/espressif/arduino-esp32) to install the necessary board support package.

2. **Connect the Hardware:**
   Connect your WT32-ETH01 to your computer using the USB to TTL adapter, and ensure the Ethernet cable is connected to a network switch or router.

### Basic Connectivity

Upload a basic sketch to verify that the module is working correctly. For example, use the "Blink" sketch to blink an onboard LED or the "Ethernet" example to check network connectivity.

## Example Projects

### Project 1: Basic Network Setup

In this project, we configure the WT32-ETH01 to connect to a local network using its Ethernet interface. This involves setting up the Ethernet library and obtaining an IP address via DHCP.

### Project 2: Sensor Integration

We will interface a temperature and humidity sensor with the WT32-ETH01 and send the data over the network. This example demonstrates how to use the I2C or SPI interfaces and transmit data to a server.

### Project 3: Data Logging

This project involves logging data from various sensors to an SD card or a remote server. We will cover how to use the built-in SD card interface and send data over HTTP or MQTT.

## Troubleshooting

Common issues and their solutions:
- **Connectivity Problems:** Check the Ethernet cable and network settings.
- **Programming Issues:** Ensure the correct board and port are selected in the Arduino IDE.
- **Library Conflicts:** Verify that all necessary libraries are installed and up to date.

## Additional Resources

- [ESP32 Arduino Core Documentation](https://docs.espressif.com/projects/arduino-esp32/en/latest/)
- [WT32-ETH01 Datasheet](https://docs.wirelesstag.net/datasheets/WT32-ETH01.pdf)
- [Arduino IDE](https://www.arduino.cc/en/Main/Software)
- [PlatformIO](https://platformio.org/)

## Contributing

If you have any examples, projects, or improvements to share, feel free to open a pull request or issue on this repository. Contributions are always welcome!

---

By sharing these examples and solutions, I hope to make it easier for others to get started with the WT32-ETH01 and unlock its full potential in their projects.
