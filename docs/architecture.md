
# System Architecture

The following diagram shows the proposed architecture of the Smart Irrigation System.

```mermaid
flowchart TD
    A["Soil Moisture Sensors"]
    B["DHT11 Sensor"]
    C["Rain Sensor"]

    A --> D["ESP32 Controller"]
    B --> D
    C --> D

    D --> E["Sensor Data Validation"]
    E --> F{"Irrigation Required?"}

    F -->|No| G["Keep Pump OFF"]
    F -->|Yes| H["XGBoost Duration Prediction"]

    H --> I["SHAP Explanation"]
    I --> J["Safety Controller"]
    J --> K["Relay / Motor Driver"]
    K --> L["Water Pump"]

    D --> M["GSM Module"]
    M --> N["Farmer Mobile Phone"]

    J --> O["Edge Fallback"]
    O --> J
```

**Note:** This represents the planned architecture. Individual components will be marked implemented after hardware and software testing.
