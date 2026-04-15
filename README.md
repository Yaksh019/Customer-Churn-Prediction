# Telco Customer Churn Prediction 📉

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![XGBoost](https://img.shields.io/badge/XGBoost-Machine%20Learning-orange.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-green.svg)
![Imbalanced-Learn](https://img.shields.io/badge/SMOTE-Class%20Imbalance-red.svg)

## 📌 Project Overview
This project focuses on predicting customer churn in the telecommunications industry. By analyzing customer demographics, account information, and service usage, the project builds a highly accurate predictive model using **XGBoost**. Special attention is given to handling class imbalance to ensure reliable prediction for both churning and retaining customers.

## 🚀 Key Features
- **Data Preprocessing:** Handled missing values (e.g., formatting `TotalCharges`) and performed label encoding for categorical variables.
- **Addressing Class Imbalance:** Applied **SMOTE** (Synthetic Minority Over-sampling Technique) to handle the 2.77:1 class imbalance ratio.
- **Predictive Modeling:** Trained an **XGBoost Classifier** to predict churn probabilities.
- **Model Evaluation:** Evaluated using accuracy scores, confusion matrices, and detailed classification reports.
- **Feature Importance:** Visualized the top driving factors behind customer churn (e.g., Contract type, Tenure, Monthly Charges).
- **Model Deployment:** Exported the trained XGBoost model and label encoders using `joblib` for future inference.

## 🛠️ Tech Stack
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** `xgboost`, `scikit-learn`
- **Imbalance Handling:** `imblearn` (SMOTE)

## 📂 Repository Structure
```text
├── data/
│   └── Telco-Customer-Churn.csv         # Raw dataset
├── models/
│   ├── customer_churn_model.pkl         # Serialized XGBoost model
│   └── churn_encoders.pkl               # Serialized Encoders
├── notebooks/
│   └── customer_churn.ipynb             # Main analysis and modeling notebook
├── .gitignore                           # Git ignore rules
├── requirements.txt                     # Environment dependencies
└── README.md                            # Project documentation
