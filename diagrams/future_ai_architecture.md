# Future AI-Enhanced Architecture

Status: Future work diagram.

This diagram shows a possible future AI-assisted extension. It is not implemented in the current repository.

```mermaid
flowchart TD
    A["Future Sensor Dataset"] --> B["Feature Extraction"]
    A1["Pulse Trends"] --> A
    A2["Immersion Duration"] --> A
    A3["IMU Motion Windows"] --> A
    A4["Optional Vision Data"] --> A
    B --> C["Future ML Experiments"]
    C --> C1["Random Forest"]
    C --> C2["XGBoost"]
    C --> C3["SVM"]
    C --> C4["LSTM"]
    C --> C5["CNN / YOLO"]
    C1 --> D["Risk Assessment Research"]
    C2 --> D
    C3 --> D
    C4 --> D
    C5 --> D
    D --> E["Alert Logic Evaluation"]
```

Future work may investigate synthetic data generated using Unity or Unreal Engine simulations and public activity recognition datasets. No implemented AI model or achieved metric is claimed.
