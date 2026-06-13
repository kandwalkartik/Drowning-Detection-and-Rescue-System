# Future ML Models

This folder is reserved for future machine learning research and experimentation.

No machine learning model is currently claimed as implemented in this repository. The current system uses threshold-based and rule-based detection because realistic drowning datasets and safe hardware simulation of drowning behavior were unavailable.

Future model directions may include:

- Random Forest for interpretable tabular sensor-feature classification.
- XGBoost for structured feature learning.
- Support Vector Machine for smaller feature-engineered datasets.
- LSTM networks for time-series sensor sequences.
- CNN-based approaches for future camera-assisted detection, where privacy and deployment constraints allow.

Planned AI pipeline:

```text
Sensor Data
  -> Feature Extraction
  -> Random Forest / XGBoost / SVM / LSTM / CNN-based approaches
  -> Drowning Risk Assessment
  -> Alert Generation
```

Future datasets may include synthetic data generated through Unity or Unreal Engine simulations and public activity recognition datasets for non-drowning motion comparison or pretraining.
