# IoT Flood Monitoring and Early Warning System

## Introduction
This repository contains the software developed for an IoT-based flood monitoring and early warning system designed for remote and resource-limited environments. The system integrates sensing, communication, and cloud-based monitoring to provide real-time flood data and alerts.

## System Overview
The system uses an ESP32 microcontroller to collect water level data from an ultrasonic sensor and battery voltage readings. The data is transmitted using a LoRa communication module to a receiver, where it is processed and visualised using a Node-RED dashboard.

Key features include:
- Real-time water level monitoring
- Long-range communication using LoRa
- Battery monitoring for energy awareness
- Data logging for historical analysis
- Email alerts when thresholds are exceeded

## Repository Structure
- `Main ESP32 Code.txt` – Contains the Arduino code for the ESP32 sensor node
- `Node-RED Flowchart.json` – Node-RED flow used for data processing and dashboard
- `Node-RED Flowchart.jpg` – Visual representation of the Node-RED system

## Requirements
To run this system, the following are required:
- ESP32 development board
- Ultrasonic sensor
- LoRa module (transmitter and receiver)
- Arduino IDE with ESP32 support
- Node-RED installed on a local machine or server

## How to Run
1. Open the ESP32 code in the Arduino IDE.
2. Install required libraries and select the correct ESP32 board.
3. Upload the code to the ESP32.
4. Set up the LoRa receiver and ensure communication is established.
5. Import the Node-RED flow file.
6. Deploy the flow and access the dashboard via a web browser.

## Technical Details
The ESP32 operates using a periodic sampling approach, where it wakes from deep sleep, takes sensor readings, transmits data, and returns to low-power mode. This ensures energy-efficient operation suitable for solar-powered deployment.

## Known Issues and Future Improvements
- The system currently uses threshold-based detection, which may limit prediction accuracy.
- Future improvements could include machine learning-based prediction models.
- Integration with cloud platforms for scalable data storage could be implemented.
- Additional sensors (e.g., rainfall, temperature) could improve system reliability.

## Academic Context
This work was developed as part of a 3rd Year Electrical and Electronic Engineering Individual Project, focusing on low-power IoT system design, embedded systems, and wireless communication.

## Repository Link for Dissertation
A link to this repository is included in the appendix of the final report, as required for evidencing software artefacts.
