# Overall System Architecture

Status: Implemented diagram.

This diagram shows the current high-level system architecture: wearable sensing, ESP32 processing, ESP-NOW/control-station communication, fog computing, and event-triggered alerting.

```mermaid
flowchart TD
    A["Pulse Sensor"] --> D["ESP32 Wearable Node"]
    B["Water Immersion Sensor"] --> D
    C["MPU6050 IMU"] --> D
    D --> E["Threshold-Based Decision Logic"]
    E --> F["ESP-NOW / Control Station Communication"]
    F --> G["Fog Computing Layer"]
    G --> H["Event-Triggered Alert"]
    H --> I["Control Station / Monitoring Unit"]
```

Note: This diagram represents the implemented academic prototype scope and does not claim machine learning or large-scale deployment.
