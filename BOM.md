# Hardware Bill of Materials

This Bill of Materials lists the main hardware components planned or used in the drowning detection system prototype. It is intended for open-source academic documentation and does not include prices, vendors, or procurement links.

| Component Name | Purpose | Interface Type | Current Status | Notes |
| --- | --- | --- | --- | --- |
| ESP32 Development Board | Main microcontroller for collecting sensor data and handling wireless communication. | GPIO, I2C, ADC, Wi-Fi/Bluetooth | Implemented | Acts as the central controller for the wearable sensing module. |
| MPU6050 IMU Sensor | Measures acceleration and orientation changes to support motion-pattern analysis. | I2C | Implemented | Useful for detecting inactivity, sudden movement, or unusual body orientation. |
| Pulse Sensor | Captures heart-rate-related physiological signals for distress-condition monitoring. | Analog ADC | Implemented | Readings may require filtering and calibration for stable wearable use. |
| Water Immersion Sensor | Detects whether the wearable module is submerged in water. | Digital or Analog GPIO | Implemented | Supports immersion detection and submersion-duration tracking. |
| Battery / Power Supply | Provides portable power for the wearable device. | Power input | Implemented | Battery selection should consider runtime, waterproofing, safety, and voltage regulation. |
| Connecting Wires | Connects sensors to the ESP32 during prototyping. | Jumper wires / headers | Implemented | Suitable for early testing; more robust connectors are recommended for wearable use. |
| Breadboard / PCB | Provides a platform for assembling and testing the circuit. | Prototyping board / custom PCB | Implemented | Breadboard is suitable for development; PCB is preferred for compact wearable deployment. |
| Enclosure or Wearable Housing | Protects electronics and supports swimmer-wearable placement. | Mechanical housing | Future | Should be waterproof, ergonomic, lightweight, and safe for aquatic environments. |

## Notes

- Component status reflects the academic prototype direction and may change as the project evolves.
- Hardware documentation should avoid private report material, personal identifiers, and unsafe deployment claims.
- The system is a work-in-progress prototype and is not a certified life-saving product.
