# IBM_Predictive-Maintenance-of-Industrial-Machinery

## Predictive Maintenance Using Machine Learning

Predictive Maintenance is a machine learning project designed to anticipate machinery failures before they occur, enabling proactive interventions, reducing unplanned downtime, and optimizing maintenance schedules. This solution uses real-time sensor data to classify different types of machine failures such as tool wear, heat dissipation issues, and power failure.

## 🚀 Project Highlights

- ✅ Accuracy > 99.5% on multi-class failure classification
- 📊 Real-time sensor data analysis (temperature, torque, speed, etc.)
- 🔄 Automated maintenance scheduling (scope)
- 📦 Scalable cloud deployment ready (IBM Cloud / IKS)
- 🧠 Handles class imbalance effectively using preprocessing techniques

---

## 📂 Dataset Overview

The dataset includes real-time operational data from a fleet of industrial machines.

| Column Name          | Description                                  |
|----------------------|----------------------------------------------|
| `udi`                | Unique identifier                            |
| `product_id`         | Identifier for the product/machine           |
| `type`               | Machine type (categorical)                   |
| `air_temperature`    | Air temperature in °C                        |
| `process_temp`       | Process temperature in °C                    |
| `rotational_speed`   | RPM (rotations per minute)                   |
| `torque`             | Torque applied to the machine                |
| `tool_wear`          | Tool wear in minutes                         |
| `target`             | Binary indicator (optional use)             |
| `failure_type`       | **Target column – type of machine failure**  |

---

## 🎯 Objective

To build a **multi-class classification model** that can predict the type of machine failure from real-time sensor inputs, thereby enabling:

- Early detection of issues
- Automated maintenance alerts
- Reduced downtime and repair costs

---

## 🧠 Machine Learning Approach

### 🔎 Preprocessing:
- Handling missing values (if any)
- Normalization of continuous sensor values
- Label encoding of categorical columns (e.g., `type`, `failure_type`)
- Dealing with class imbalance using:
  - SMOTE (Synthetic Minority Oversampling Technique)
  - Class weights in model training

### 📈 Model(s) Used:
- Random Forest Classifier
- XGBoost
- Deep Learning models (LSTM / CNN) – for advanced time-series modeling *(future scope)*

### 🧪 Evaluation Metrics:
- Accuracy
- Precision, Recall, F1-Score (per class)
- Confusion Matrix

---

