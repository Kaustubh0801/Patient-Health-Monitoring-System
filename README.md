# Patient-Health-Monitoring-System
This project outlines the creation of an IoT-Based Patient Health Monitoring System using the ESP32 Web Server, which allows real-time monitoring of patient health parameters like heart rate, blood oxygen levels, and body temperature. Here's a breakdown of the project:

## Overview

The system is designed for continuous monitoring of patients' health, particularly for the elderly, whose vital signs must be tracked periodically. The device uses sensors to measure:\n

Heart rate and blood oxygen level using the MAX30100/102 Pulse Oximeter.\n
Body temperature using the DS18B20 Temperature Sensor.\n
Room temperature and humidity with the DHT11 Sensor.

## Components

The system requires the following components:

ESP32 Board – microcontroller for running the web server.\n
MAX30100 Pulse Oximeter Sensor – to measure heart rate (BPM) and oxygen level (SpO2).\n
DS18B20 Temperature Sensor – for body temperature measurement.\n
DHT11 Sensor – for room temperature and humidity monitoring.\n
Resistors and connecting wires for circuit assembly.

## Working

The project works by interfacing these sensors with the ESP32, which collects the data and displays it on a web server. Users can monitor the patient's vital signs remotely over the network. Here's how the individual components function:

The MAX30100 sensor uses infrared light to detect oxygen levels in the blood and heart rate.
The DS18B20 sensor is digital, providing precise body temperature readings.
The DHT11 sensor measures room temperature and humidity, ensuring a comfortable environment for the patient.

## Code Explanation

The ESP32 runs a web server where patient data is updated in real-time. The source code utilizes libraries for interfacing with the sensors and handling web requests. The data is processed and displayed on an HTML page hosted by the ESP32, with specific styling for better readability.

## Key Features

Real-time monitoring of vital parameters.\n
Remote access via a web server.\n
Periodic data reporting with clear indicators for BPM, SpO2, and temperatures.

This project could be expanded with additional features like alerts or notifications based on abnormal readings, making it a robust solution for patient health monitoring.
