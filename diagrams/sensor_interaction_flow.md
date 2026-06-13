# Sensor Interaction Flow

Status: Implemented diagram.

This diagram shows how the current sensors contribute to the threshold-based detection logic.

```mermaid
flowchart TD
    A["Pulse Sensor"] --> A1["Physiological Signal Reading"]
    B["Water Immersion Sensor"] --> B1["Submersion State"]
    C["MPU6050 IMU"] --> C1["Motion and Orientation Data"]
    A1 --> D["ESP32 Sensor Collection"]
    B1 --> D
    C1 --> D
    D --> E["Filtering / Basic Validation"]
    E --> F["Threshold and Rule Evaluation"]
    F --> G{"Possible Drowning Risk?"}
    G -- "No" --> H["Continue Monitoring"]
    G -- "Yes" --> I["Event-Triggered Alert"]
```

Note: The interaction flow is rule-based and does not claim AI-based sensor fusion.
