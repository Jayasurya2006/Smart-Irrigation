# Machine Learning Module

## Overview

The proposed Smart Irrigation System uses machine learning to support intelligent irrigation decisions based on sensor data.

The planned approach uses a two-stage XGBoost architecture.

## 1. Stage One — Irrigation Requirement Classification

**Model:** XGBoost Classifier

Input features:
- Soil moisture readings
- Temperature
- Humidity
- Rain detection

Output:
- 0 — Irrigation not required
- 1 — Irrigation required

## 2. Stage Two — Irrigation Duration Prediction

**Model:** XGBoost Regressor

This model is intended to estimate the irrigation duration when irrigation is required.

Input:
- Validated sensor readings
- Relevant environmental conditions

Output:
- Estimated irrigation duration

## 3. Explainable AI — SHAP

SHAP (SHapley Additive exPlanations) is planned to explain model predictions.

It can help identify:
- Which sensor values influence irrigation decisions.
- Which environmental conditions affect predictions.
- How individual features contribute to model outputs.

## 4. Data Processing

Planned tools:
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- SHAP

## 5. Model Evaluation

The models will be evaluated using suitable metrics.

**Classification:**
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

**Regression:**
- MAE
- RMSE
- R² score

Time-based validation will be considered to reduce data leakage.

## 6. Future Improvements

- Collect real sensor data.
- Train and validate both models.
- Compare predictions with actual irrigation requirements.
- Evaluate water consumption.
- Explore deployment on edge hardware.

## Current Status

The machine-learning architecture is proposed. Model training, performance evaluation and hardware integration will be documented after implementation.
