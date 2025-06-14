
# 🛠️ Machine Failure Prediction - README

## 📁 Project Title:
**Machine Failure Prediction using Random Forest**

---

## 📋 Description:
This project aims to predict machine failures in advance using sensor data collected from machines. The dataset includes readings like temperature, air quality, VOCs, electrical current, etc. A machine learning model is trained to classify whether a machine is likely to fail (`1`) or not (`0`).

---

## 🧾 Dataset Overview:
**Filename:** `data (1).csv`

| Column        | Description |
|---------------|-------------|
| `footfall`    | Number of people or objects passing by the machine |
| `tempMode`    | Temperature setting of the machine |
| `AQ`          | Air Quality index |
| `USS`         | Ultrasonic sensor value |
| `CS`          | Current sensor value |
| `VOC`         | Volatile Organic Compound level |
| `RP`          | Rotational position or RPM |
| `IP`          | Input pressure |
| `Temperature` | Operating temperature |
| `fail`        | Target variable (1 = machine failed, 0 = working) |

---

## 📌 Objective:
To build a machine learning model that predicts the `fail` column using the sensor features, helping to prevent costly machine downtimes.

---

## 🛠️ Technologies Used:
- Python 3.x
- pandas
- scikit-learn
- matplotlib
- seaborn

---

## 🧠 Machine Learning Model:
**Algorithm:** Random Forest Classifier  
**Train/Test Split:** 80/20  
**Accuracy Achieved:** ~87.8%

---

## 📊 Feature Importance Plot:
The Random Forest model ranks each sensor feature based on its contribution to predictions.  
📁 File: `feature_importance_plot.png`

---

## 📁 File Structure:
```
├── data (1).csv                 # Dataset
├── feature_importance_plot.png # Feature importance bar chart
├── machine_failure_model.py    # Python code for model training
├── README.md                   # This file
```

---

## 🚀 How to Run:
1. Install required libraries:
   ```bash
   pip install pandas scikit-learn matplotlib seaborn
   ```

2. Run the script:
   ```bash
   python machine_failure_model.py
   ```

3. View output in the terminal and graph in `feature_importance_plot.png`.

---

## ✅ Future Improvements:
- Try different models (e.g., XGBoost, SVM).
- Perform hyperparameter tuning.
- Build a real-time dashboard or API with Flask.
- Implement alerting or monitoring based on predictions.
