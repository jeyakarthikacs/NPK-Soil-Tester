# NPK Sensor System Using Arduino and OLED Display
This repository contains the code for a Nitrogen, Phosphorous, and Potassium (NPK) Sensor System using an Arduino. The system reads the NPK values from a sensor and displays them on an OLED screen. This project helps monitor soil nutrients, providing essential data for farming and agriculture.

## Table of Contents
- Introduction
- Features
- Technologies Used
- Hardware Requirements
- Setup Instructions
- Output

## Introduction
The NPK Sensor System reads soil nutrient levels (Nitrogen, Phosphorous, and Potassium) using a sensor module and displays the values on an OLED screen. It communicates with the sensor over Modbus using a software serial interface. The data collected is essential for determining soil health and making informed decisions in agriculture.

## Features
- Reads NPK Values: Displays Nitrogen, Phosphorous, and Potassium levels in mg/kg.
- OLED Display: Shows real-time data on a 128x64 OLED screen.
- Modbus Communication: Communicates with the NPK sensor via Modbus protocol.
- Serial Monitoring: Outputs sensor values over the serial monitor.
  
## Technologies Used
- Arduino Uno/Nano: Microcontroller to run the system.
- Adafruit SSD1306 Library: For controlling the OLED display.
- Adafruit GFX Library: Provides the graphics for the OLED.
- Modbus Communication: Communicates with the NPK sensor using a SoftwareSerial interface.
  
## Hardware Requirements
- NPK Sensor: For measuring Nitrogen, Phosphorous, and Potassium levels.
- Arduino Uno/Nano: Microcontroller to run the code.
- 128x64 OLED Display: To display NPK values.
- Jumper Wires: For connections.
  
## Setup Instructions

**Clone the Repository:**

      git clone https://github.com/your-username/npk-sensor-system.git
      cd npk-sensor-system

**Hardware Setup:**

- Connect the NPK sensor to the Arduino via the TX/RX pins using a SoftwareSerial interface.
- Connect the OLED display to the I2C pins of the Arduino.
- Ensure that the power and ground connections for the sensor and OLED are properly connected.
-Library Installation: Install the required libraries in the Arduino IDE:

      Adafruit_GFX.h
      Adafruit_SSD1306.h
      SoftwareSerial.h
  
- To install the libraries:

Go to Sketch > Include Library > Manage Libraries...
Search for "Adafruit GFX" and "Adafruit SSD1306", and install both.
- Upload the Code: Open the npk_sensor.ino file in the Arduino IDE, select the correct board and port, and upload the code.
- Serial Monitor: Open the Serial Monitor to observe the NPK readings (set to 9600 baud).

## Output

Nitrogen: The nitrogen content in mg/kg.
Phosphorous: The phosphorous content in mg/kg.
Potassium: The potassium content in mg/kg.
The data is displayed on both the OLED screen and the serial monitor.

