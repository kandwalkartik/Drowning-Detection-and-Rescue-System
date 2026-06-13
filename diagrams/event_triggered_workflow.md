# Event-Triggered Drowning Detection Workflow

Status: Implemented diagram.

This flowchart describes the current rule-based detection workflow. The system evaluates sensor readings using thresholds and triggers alerts only when configured risk conditions are satisfied.

```mermaid
flowchart TD
    A["Start Monitoring"] --> B["Read Pulse Sensor"]
    B --> C["Read Water Immersion Sensor"]
    C --> D["Read MPU6050 IMU"]
    D --> E["Validate and Filter Sensor Values"]
    E --> F{"Immersion Detected?"}
    F -- "No" --> A
    F -- "Yes" --> G["Measure Immersion Duration"]
    G --> H["Evaluate Pulse Threshold"]
    H --> I["Evaluate Motion / Orientation Rules"]
    I --> J{"Combined Risk Condition Met?"}
    J -- "No" --> A
    J -- "Yes" --> K["Generate Distress Event"]
    K --> L["Send Alert to Control Station"]
    L --> M["Monitoring / Response Action"]
```

Note: This workflow does not use implemented machine learning.
