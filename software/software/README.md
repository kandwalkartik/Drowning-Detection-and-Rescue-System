# Software

This folder organizes the software side of the drowning detection system. The current project direction is based on threshold-based and rule-based detection using wearable sensor readings. Future folders are included for planned AI, communication, and fog computing extensions.

## Structure

| Folder | Purpose |
| --- | --- |
| `esp32_firmware/` | ESP32 firmware for reading sensors and transmitting data. |
| `sensor_processing/` | Sensor filtering, calibration, feature preparation, and rule inputs. |
| `alert_system/` | Alert generation logic and notification interface planning. |
| `communication/` | Wireless communication, MQTT, and message-format documentation. |
| `fog_layer/` | Local fog-node processing and low-latency decision logic. |
| `future_ml_models/` | Planned machine learning extensions for future research. |

Software added here should clearly distinguish implemented threshold-based logic from future AI proposals. No completed machine learning implementation or validated ML accuracy is claimed in this repository.
