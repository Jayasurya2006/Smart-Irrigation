# ESP32 Firmware

## Overview

The ESP32 acts as the central controller of the Smart Irrigation System. It collects environmental sensor readings, validates the input data and manages irrigation operations.

## Development Environment

- Microcontroller: ESP32
- Programming Language: Embedded C/C++
- IDE: Arduino IDE
- Communication: UART for GSM module

## Firmware Responsibilities

1. Initialize connected sensors.
2. Read soil moisture values.
3. Collect temperature and humidity from DHT11.
4. Detect rainfall using the rain sensor.
5. Validate sensor readings.
6. Determine irrigation requirements.
7. Control the pump through a suitable driver.
8. Communicate with the GSM module.

## Planned Firmware Workflow

```text
START
  |
Initialize ESP32 and sensors
  |
Read sensor values
  |
Validate sensor readings
  |
Check irrigation requirement
  |
Control pump safely
  |
Send GSM notification
  |
Repeat monitoring cycle
```

## Safety Features

- Prevent pump activation when sensor data is invalid.
- Use a maximum irrigation duration limit.
- Provide a manual pump shutdown mechanism.
- Handle sensor disconnection and communication failures.

## Future Implementation

- Sensor calibration.
- GSM SMS command handling.
- Machine learning model integration.
- Edge-based fallback operation.
- Tamil SMS notifications.

## Current Status

Firmware development and hardware integration are in progress. Actual source code and pin configurations will be uploaded after implementation and testing.
