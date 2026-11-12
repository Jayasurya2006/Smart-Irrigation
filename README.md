# Smart Irrigation System Using ESP32

An IoT-based smart irrigation project designed to monitor soil and environmental conditions and support intelligent water management in agriculture.

## Project Overview

This project explores an automated irrigation system using an ESP32 microcontroller and multiple sensors. The system collects field data and uses a machine-learning-based decision approach to determine whether irrigation is required.

The proposed design also includes farmer communication through GSM-based SMS notifications.

## Objectives

- Monitor soil moisture and environmental conditions.
- Reduce unnecessary water usage.
- Explore machine learning for irrigation decisions.
- Provide a practical and affordable solution for farmers.
- Enable remote communication through GSM.

## Proposed System Architecture

1. **Sensor Layer:** Capacitive soil-moisture sensors, DHT11 and rain sensor.
2. **Controller Layer:** ESP32 collects and processes sensor readings.
3. **Data Validation:** Checks sensor readings and identifies invalid data.
4. **Machine Learning:** XGBoost-based irrigation decision and duration prediction.
5. **Explainable AI:** SHAP to understand model predictions.
6. **Actuation:** Pump control through a suitable driver or relay.
7. **Communication:** GSM module for SMS-based farmer notifications.

## Hardware Components

| Component | Purpose |
|---|---|
| ESP32 | Main controller |
| Capacitive soil-moisture sensors | Soil moisture monitoring |
| DHT11 | Temperature and humidity |
| Rain sensor | Rain detection |
| SIM800L GSM module | SMS communication |
| Relay / motor driver | Pump control |
| Water pump | Irrigation |

*Final component selection and wiring will be documented as the prototype is developed.*

## Proposed Technology Stack

- **Embedded:** ESP32, Embedded C/C++, Arduino IDE
- **Machine Learning:** Python, XGBoost, Scikit-learn
- **Explainable AI:** SHAP
- **Data Processing:** Pandas, NumPy
- **Communication:** GSM / SMS

## Machine Learning Approach

The planned two-stage model consists of:

- **Stage 1:** Classification — predict whether irrigation is required.
- **Stage 2:** Regression — estimate irrigation duration when irrigation is required.

SHAP will be explored to explain the model's predictions.

## Project Status

**Development in progress.**

The architecture and implementation plan are being documented. Hardware integration, model training and field testing will be updated as they are completed.

## Future Enhancements

- Tamil SMS notifications for farmers.
- Voice-call alerts and IVR support.
- Sensor fault detection.
- Edge-based fallback operation.
- Field testing and water-consumption evaluation.

## Repository Structure

```text
Smart-Irrigation/
├── README.md
├── images/
├── docs/
├── hardware/
├── firmware/
├── machine-learning/
├── dataset/
└── demo/
```

## Project Goal

To explore an affordable, intelligent and farmer-friendly irrigation solution using IoT and machine learning.
