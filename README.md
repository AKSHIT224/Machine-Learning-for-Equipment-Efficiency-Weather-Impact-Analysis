# 🚛 Machine Learning for Equipment Efficiency & Weather Impact Analysis
 
## Akshit Bhandari (Machine Learning Analyst)

---

## 📌 Project Overview

This project focuses on predicting two major operational challenges using machine learning:
1. *Fuel delivery delays* caused by extreme weather conditions.
2. *Equipment failure risks* based on usage history and operational metadata.

The system is designed for *Innoflow’s KORIKI and SAND OCEAN substations*, aiming to improve scheduling, reduce downtime, and support proactive maintenance through predictive analytics.

---

## 🎯 Objectives

- Predict whether a fuel delivery will experience long delays due to environmental factors.
- Estimate equipment failure risks using historical fuel dispensing and status records.
- Analyze correlations between weather patterns and operational performance.
- Provide actionable insights to support smarter decision-making for scheduling and resource allocation.

---

## 📂 Project Components

### 1️⃣ Fuel Delivery Delay Prediction

- *Target*: Predict if a delivery will run longer than 365 minutes.
- *Key Features*: Volume, Air Temperature, Hour of Day, Day of Week, Weekend Indicator.
- *Engineering*:
  - Converted timestamps and extracted time-based features.
  - Calculated delay labels using average delivery duration thresholds.
- *Model*: Random Forest Classifier  
- *Performance*:  
  - Accuracy: *97.28%*  
  - High precision/recall for both delayed and non-delayed classes.
- *Insights*:
  - Highest delays during extreme cold (< -16°C) and early hours (12 AM – 8 AM).
  - Midday deliveries in moderate temperatures (12°C–20°C) showed the best performance.

---

### 2️⃣ Equipment Failure Prediction

- *Target*: Classify equipment as failed or not failed based on its status (DECOMM or OUTS).
- *Key Features*: Equipment Make/Model, Days Since Last Use, Usage Frequency, Total Volume Dispensed.
- *Engineering*:
  - Aggregated dispensing records to calculate usage frequency.
  - Added binary failure labels and handled class imbalance with *SMOTE*.
- *Model*: Random Forest with SMOTE  
- *Performance*:  
  - Accuracy: *93%*
  - Balanced F1 scores and improved recall for rare failure cases.
- *Insights*:
  - *Emulsion Chargers* had the highest risk.
  - Light Vehicles had moderate risk but the largest equipment count (n=254).

---

## 📊 Visualization Highlights

- Delivery delays peak in winter months and extreme temperatures.
- Equipment failure likelihood increases with certain makes/models and usage patterns.
- Delay probability decreases with increased delivery volume and milder temperatures.

---

## 🧠 Responsible AI Practices

- *Fairness*: Models were validated to avoid geographic or time-based biases.
- *Transparency*: Feature importance metrics were shared to aid interpretability.
- *Privacy*: No customer data was used. Only anonymized operational and weather data.

---

## 💻 Tools & Technologies

- Python, pandas, scikit-learn, matplotlib, seaborn
- Random Forest, SMOTE (Synthetic Minority Oversampling)
- Jupyter Notebook

---

For the files related to this project, due to privacy policy of my client, I was unable to upload it.  

---

## 📞 Contact

*Akshit Bhandari*  
📧 abhandari78@norquest.ca  
📞 +1 (437) 970-9974

---
