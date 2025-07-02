# Diabetes Classification: Machine Learning Project

This project builds and evaluates machine learning models to predict whether a patient has diabetes using a set of medical and demographic features. It includes extensive preprocessing, model training, evaluation, and hyperparameter tuning.

---

## 📊 Project Overview

The goal of this project is to accurately predict the presence of diabetes using patient health metrics, such as glucose levels, BMI, blood pressure, and more.

### Dataset
- **Source:** Pima Indians Diabetes Dataset
- **Rows:** 768 observations
- **Features:**
  - Pregnancies
  - Glucose
  - Blood Pressure
  - Skin Thickness
  - Insulin
  - BMI
  - Diabetes Pedigree Function
  - Age
  - Outcome (Target Variable)

---

## 🔎 Key Steps

### 1. Data Cleaning & Preprocessing
- Replaced zero values in non-logical features (like glucose and BMI) with the feature’s median.
- Standardized features for all models to ensure fair comparisons.

### 2. Exploratory Data Analysis
- Checked class imbalance: ~65% non-diabetic, ~35% diabetic.
- Visualized feature distributions and correlations.

### 3. Model Training
Tested the following classifiers:
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Random Forest**
- **Decision Tree**
- **Naïve Bayes**

### 4. Model Evaluation
- **Metrics:** Accuracy, Precision, Recall, F1-Score, ROC-AUC
- Performed hyperparameter tuning using cross-validation.
- KNN achieved the highest performance with a balanced trade-off between recall and precision.

---

## ⚙️ Final Model
- **Selected Model:** K-Nearest Neighbors
- **Key Performance Metrics:**
  - Accuracy: ~77%
  - ROC-AUC: ~82%
- Balanced detection of positive diabetes cases with low false positives.

---

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## 👥 Contributors
- Hira Stanley
- Yumeng Li
- Paul Pham
- Michelle Zhu
- Iris Huang
- 
---

## ✅ Next Steps (Future Improvements)
- Address remaining class imbalance using SMOTE or other resampling techniques.
- Explore additional models like XGBoost or ensemble stacking.
- Incorporate clinical domain expertise for further feature engineering.
