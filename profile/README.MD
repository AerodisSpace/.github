# AerodisSpace: Streaming Platform for Model Aviation Enthusiasts

## Project Overview

AerodisSpace is a cutting-edge streaming platform tailored for model aviation enthusiasts. It provides a unique space for both hobbyists and professionals in the field to join specific channels and follow model aircraft flights in real-time. The platform offers two primary viewing modes: FPV (First-Person View) video and tracking via sensory data.

## Key Features

### Real-time Data

- **Supported Sensors**: AerodisSpace captures and streams real-time data from various sensors equipped on the model aircraft, including GPS, gyroscope, accelerometer, and others that users choose to share.
- **Data Storage**: Users can store their flight data, enabling the creation of datasets. These datasets can be used to train machine learning models for the purpose of automating model aircraft stabilization and configuration.

### LoRa Technology Integration

- **LoRa Module**: If the flight device is equipped with a LoRa module, users can integrate it with the Helium network by Solana, leveraging LoRa technology for IoT (Internet of Things) applications.

## Employed Technologies

### Backend

- **Languages and Frameworks**: Utilizes Rust, rocket-rs, scylladb, redis, and websockets for real-time data communication.

### Embedded Systems

- **Technologies**: Rust and C/C++.
	- **Hardware Support**: Compatible with ESP32, ESP8266, Arduino (any).
- **Functionality**: The provided code simplifies integration, requiring users to only update the WiFi SSID and password fields in a text editor, along with a platform-generated token.

### Frontend/Cross-Platform App

- **Technologies**: The user interface is developed with Vue and TypeScript, employing WASM (WebAssembly) for Rust components integration and styled with Tailwind. The Tauri framework is used to create cross-platform applications that operate on Android, Windows, and Linux, offering an easy-to-use UI. Users can configure their model aircraft settings, such as maximum motor speed, maximum servo angles, positions, and their pins on the embedded system.

## Basic Operation:

1. Register an account on the platform.
2. Create and configure a model aircraft on the platform.
3. Save and generate the model aircraft's token.
4. Download the embedded code from GitHub.
5. Configure the WiFi SSID and PASSWORD, and input the model aircraft's token in the code.
6. Once set up, power on the model aircraft/embedded system, and it will be configured.
7. The system will report its online status every minute.
8. If online, start a broadcast on the platform (options include data and video streaming).
