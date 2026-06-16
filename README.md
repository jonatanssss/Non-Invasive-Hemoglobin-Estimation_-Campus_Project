# Non-Invasive Hemoglobin Estimation from Conjunctival Images

## Overview

This project explores a non-invasive approach for estimating hemoglobin (Hb) concentration using conjunctival images and machine learning techniques.

The objective is to reduce dependence on invasive blood sampling by extracting clinically relevant colorimetric features from conjunctival images and predicting hemoglobin concentration in real time.

## Dataset

- Eyes Defy Anemia Dataset
- Conjunctival images with corresponding laboratory hemoglobin measurements

## Methodology

### Image Processing

- Conjunctival ROI extraction
- Advanced masking
- Illumination normalization
- Color space transformation

### Feature Engineering

Features extracted from:

- RGB color space
- CIELAB color space
- HSV color space
- Clinical color indices

Examples:

- Pallor Index
- Redness Index
- Delta-E Analysis

### Machine Learning Models

1. Polynomial Ridge Regression (PBC)
2. Gradient Boosting Soft Sensor (IC)

## Results

### Gradient Boosting Soft Sensor

| Metric | Value |
|----------|----------|
| MAE | 0.645 g/dL |
| RMSE | 0.819 g/dL |
| R² | 0.856 |
| Sensitivity | 83.3% |
| Specificity | 88.0% |
| Diagnostic Accuracy | 86.0% |

### Polynomial Ridge Regression

| Metric | Value |
|----------|----------|
| MAE | 1.508 g/dL |
| RMSE | 1.872 g/dL |
| R² | 0.248 |

## Additional Analysis

- Bland-Altman Analysis
- Calibration Curve
- Pearson Correlation Analysis
- Gender Stratification Analysis

## Technologies

- Python
- OpenCV
- NumPy
- Pandas
- Scikit-Learn
- Matplotlib
- Scikit-Image

## Author

Jonatan Pardamean Manurung
Physics Undergraduate | Machine Learning & Computer Vision Enthusiast

## Repository Structure

```text
.
├── README.md
├── requirements.txt
└── notebooks
    └── hemoglobin_estimation.ipynb
