# Chinese Brush – Air Writing System

Chinese Brush is an air-writing system that creates Chinese characters through hand movements, simulating the characteristics of traditional Chinese brush calligraphy in a digital environment.

The project focuses on predicting brush-stroke thickness along the **Z-axis** while preserving the original **X/Y coordinates** using **Temporal Convolutional Networks (TCNs)**.

## Key Contributions

- Reimplemented and compared five TCN architectures for sequence-to-sequence Z-axis prediction:
  - Basic TCN
  - Attention TCN
  - WaveNet-style TCN
  - Residual TCN
  - Multi-scale TCN
- Explored variable-length sequences using post-padding and masking.
- Evaluated only valid timesteps to ensure fair performance measurement.
- Predicted brush-stroke thickness while preserving the original X/Y coordinates.

## Model Evaluation

The five architectures were evaluated on a held-out test set using four metrics:

| Metric | Description |
|---|---|
| **MAE** | Mean Absolute Error |
| **RMSE** | Root Mean Squared Error |
| **DTW** | Dynamic Time Warping |
| **SSIM** | Structural Similarity Index Measure |

## Objective

The goal is to investigate and compare different temporal modeling approaches to generate more natural and expressive digital Chinese brush strokes.

## Technologies

- Python
- Deep Learning
- Temporal Convolutional Networks (TCNs)
- Sequence-to-Sequence Modeling
- Time-Series Evaluation
