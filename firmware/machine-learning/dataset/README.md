# Dataset Documentation

## Overview

This directory is intended to store sensor readings collected from the ESP32 Smart Irrigation System.

## Planned Dataset Features

| Column | Description |
|---|---|
| timestamp | Date and time of measurement |
| soil_moisture_1 | First soil moisture reading |
| soil_moisture_2 | Second soil moisture reading |
| soil_moisture_3 | Third soil moisture reading |
| temperature | Temperature in Celsius |
| humidity | Relative humidity percentage |
| rain_status | Rain detection status |
| irrigation_required | Target classification label |
| irrigation_duration | Target duration in seconds |

## CSV Format

A future dataset may use the following header:

```csv
timestamp,soil_moisture_1,soil_moisture_2,soil_moisture_3,temperature,humidity,rain_status,irrigation_required,irrigation_duration
```

## Data Collection Guidelines

- Record actual sensor readings with timestamps.
- Calibrate soil moisture sensors.
- Document missing or invalid readings.
- Record irrigation decisions and actual pump duration.
- Collect data under different weather and soil conditions.

## Important

No experimental measurements are included yet. Actual data will be added after sensor integration and field testing.
