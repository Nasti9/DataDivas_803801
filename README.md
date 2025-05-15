# Anomaly Detetction - REPLY 
**Team Members:** Anastasia Farinaro (803801) , Gaia D'Amico, Alessia Lorenzini

---

## Section 1 – Introduction

This project focuses on the development of an anomaly detection system applied to a time-series dataset. The dataset consists of daily records of system alarms, including attributes such as Code_ID, Timestamp, Number of Transactions, Time Min, Time Max, Number of Retries, and Number of Wrong Transactions. These features capture essential aspects of transactional system behavior over time.

The objective is to design and implement a pipeline that integrates forecasting models with anomaly detection techniques to identify unusual patterns or behaviors that deviate from expected trends.

The ultimate goal is to detect deviations in system behavior at an early stage, in order to prevent potential failures or ambiguous activity. Early identification of such anomalies is crucial for maintaining operational reliability, as well as for uncovering possible system malfunctions or fraudulent actions.


---

## Section 2 – Methods

We followed a sequential pipeline composed of four main phases: Exploratory Data Analysis (EDA), Data Augmentation, Forecasting, and Anomaly Detection.
For each step, we tested different approaches and selected the one that gave the best results. This allowed us not to settle for the first attempt, but to explore multiple options and make more informed choices along the way.

### 2.1 Exploratory Data Analysis (EDA) ###

We conducted a time-based exploratory analysis of the numerical features. 
The total transactions showed strong and repeatable daily patterns, making them suitable for forecasting. Failed transactions were more volatile but followed similar peak-hour trends, while retry attempts were extremely sparse, with localized spikes suggesting critical anomalies.  




