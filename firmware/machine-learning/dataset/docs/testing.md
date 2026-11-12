# Testing and Validation

## Overview

This document describes the planned testing procedure for the ESP32 Smart Irrigation System.

## 1. Sensor Testing

- Verify soil moisture sensor readings.
- Compare readings under dry and wet soil conditions.
- Verify DHT11 temperature and humidity readings.
- Test rain sensor detection.
- Check sensor disconnection and invalid readings.

## 2. ESP32 Testing

- Verify sensor initialization.
- Check periodic data acquisition.
- Validate sensor data processing.
- Test communication between ESP32 and GSM module.

## 3. Machine Learning Testing

- Evaluate irrigation requirement classification.
- Evaluate irrigation duration predictions.
- Measure accuracy, precision, recall and F1-score.
- Calculate MAE and RMSE for regression.
- Inspect model explanations using SHAP.

## 4. Pump Control Testing

- Verify relay or motor driver operation.
- Test pump activation and deactivation.
- Check maximum irrigation duration.
- Verify manual emergency shutdown.
- Test behavior when sensor readings are invalid.

## 5. GSM Communication Testing

- Verify network registration.
- Test SMS delivery.
- Test START, STOP and STATUS command handling if implemented.
- Check communication failure handling.

## 6. Field Validation

Future field testing will evaluate:

- Soil moisture variation.
- Irrigation decisions.
- Actual water consumption.
- Pump operating duration.
- System reliability under different weather conditions.

## Test Results

Actual test results, screenshots, measurements and observations will be added after testing.

## Current Status

This document describes the planned validation process. It does not represent completed test results.
