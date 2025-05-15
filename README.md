# Anomaly Detetction - REPLY 
**Team Members:** Anastasia Farinaro (803801) , Gaia D'Amico, Alessia Lorenzini

---

## Section 1 – Introduction

This project focuses on the development of an anomaly detection system applied to a time-series dataset. The dataset consists of daily records of system alarms, including attributes such as Code_ID, Timestamp, Number of Transactions, Time Min, Time Max, Number of Retries, and Number of Wrong Transactions. These features capture essential aspects of transactional system behavior over time.

The objective is to design and implement a pipeline that integrates forecasting models with anomaly detection techniques to identify unusual patterns or behaviors that deviate from expected trends.

The ultimate goal is to detect deviations in system behavior at an early stage, in order to prevent potential failures or ambiguous activity. Early identification of such anomalies is crucial for maintaining operational reliability, as well as for uncovering possible system malfunctions or fraudulent actions.


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

