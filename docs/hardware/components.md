# Hardware Components

## 1. ESP32 Development Board
- Main controller of the irrigation system.
- Collects sensor readings.
- Processes data and controls irrigation operations.
- Supports Wi-Fi and Bluetooth connectivity.

## 2. Capacitive Soil Moisture Sensors
- Measure moisture levels in the soil.
- Help determine whether plants need water.
- Multiple sensors can monitor different soil locations.

## 3. DHT11 Sensor
- Measures surrounding temperature and humidity.
- Provides environmental information for irrigation decisions.

## 4. Rain Sensor
- Detects rainfall conditions.
- Helps avoid unnecessary irrigation during rain.

## 5. SIM800L GSM Module
- Enables communication through a mobile network.
- Intended for sending SMS notifications to farmers.
- Requires a suitable power supply and compatible SIM/network support.

## 6. Relay Module / Motor Driver
- Acts as the switching interface between the ESP32 and water pump.
- Provides controlled pump operation.
- Must be selected according to the pump's voltage and current requirements.

## 7. Water Pump
- Supplies water to the plants.
- Operated through the relay or suitable motor driver.

## Hardware Integration Plan

1. Connect soil moisture sensors to ESP32 analog inputs.
2. Connect DHT11 using a suitable digital GPIO.
3. Connect the rain sensor to a suitable ESP32 input.
4. Interface the GSM module with ESP32 using UART.
5. Connect the pump through a properly rated driver or relay.
6. Test each component independently before full integration.

## Safety Notes
- Never connect a water pump directly to an ESP32 GPIO.
- Use a suitable external power supply for the pump.
- Check the SIM800L power requirements before connecting it.
- Ensure a common ground where required.
- Keep electronics protected from water.

## Current Status

This document describes the planned hardware configuration. Actual pin connections, component specifications and photographs will be added after confirming the physical prototype.
