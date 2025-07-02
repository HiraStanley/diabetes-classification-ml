# Diabetes Classification: Machine Learning Project

This project builds and evaluates machine learning models to predict whether a patient has diabetes using a set of medical and demographic features. It includes extensive preprocessing, model training, evaluation, and hyperparameter tuning.

---

## 📊 Project Overview

Diabetes significantly impacts hospitalization rates and emergency department visits in the United States. Early identification of at-risk patients can improve patient outcomes and reduce unnecessary healthcare costs.
The goal of this project is to accurately predict the presence of diabetes using patient health metrics, such as glucose levels, BMI, blood pressure, and more.

### Business Value
- Improve diagnostic accuracy.
- Reduce missed diabetes cases.
- Enhance preventative healthcare.

## 📂 Dataset

- **Source:** Behavioral Risk Factor Surveillance System (BRFSS) survey  
- **Collected by:** CDC  
- **Year:** 2015  
- **Size:** ~69,000 survey responses

### Key Features
- High Blood Pressure  
- Cholesterol Level  
- BMI  
- General Health Rating  
- Age Group  
- Education Level  
- Income Level  
- Mental and Physical Health Days
  
---

## 🔎 Key Steps

### 1. Data Cleaning & Preprocessing
- Replaced zero values in non-logical features (like glucose and BMI) with the feature’s median.
- Standardized features for all models to ensure fair comparisons.
- Mapped outliers to bins for BMI, mental health, physical health, age, education, and income.

### 2. Exploratory Data Analysis
- Checked class imbalance: ~65% non-diabetic, ~35% diabetic.
- Visualized feature distributions.
- Identified strong correlations with high blood pressure, cholesterol, and BMI.

### 3. Model Training

### Models Tested
- Logistic Regression
- K-Nearest Neighbors
- Decision Trees
- Random Forest
- Gradient Boosting
- XGBoost

### Final Model
- **Best Model:** Gradient Boosting
- **Performance:**
  - F1-Score: **0.7734**
  - Recall: **0.8041**
  - Precision: ~74%

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
  
---

## ✅ Next Steps (Future Improvements)
- Address remaining class imbalance using SMOTE or other resampling techniques.
- Explore additional models like XGBoost or ensemble stacking.
- Incorporate clinical domain expertise for further feature engineering.
