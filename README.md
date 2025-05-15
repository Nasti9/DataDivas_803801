# Anomaly Detetction - REPLY 
**Team Members:** Anastasia Farinaro, Gaia D'Amico, Alessia Lorenzini

---

## Section 1 – Introduction

This project aims to [briefly state the objective of the project, e.g., develop a machine learning-based anomaly detection model for time series data collected from transaction logs]. Our motivation stems from the need to [add your motivation: e.g., identify deviations in system behavior early to prevent potential failures or fraudulent activity]. By leveraging recent advances in forecasting models and unsupervised learning, our system enables proactive monitoring and early warning capabilities.

---

## Section 2 – Methods

Our pipeline integrates a combination of time-series forecasting and anomaly detection techniques. The workflow consists of the following stages:

1. **Data Cleaning and Preprocessing:** Handling of missing values, feature engineering (lags, rolling averages).
2. **Forecasting Models:** We trained both LSTM-based models and XGBoost regressors on enriched time-series features.
3. **Anomaly Detection:** Residual-based anomaly scoring using statistical thresholds and Local Outlier Factor (LOF).
4. **Evaluation and Visualization:** Metrics and visual outputs support interpretation of anomalies.

**Design Choices:**
- We chose LSTM for its ability to capture temporal dependencies and XGBoost for structured feature modeling.
- LOF was selected for its robustness in identifying local density anomalies.
- Synthetic data was generated using [SMOTE/TimeGAN, etc.] to augment underrepresented patterns and enhance generalization.

**Environment Setup:**
To recreate the environment, use the following:
```bash
conda env export > environment.yml

