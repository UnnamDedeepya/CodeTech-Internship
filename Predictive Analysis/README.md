
# 🧠 Diabetes Prediction – Machine Learning Model  
### 💼 Internship Task: Predictive Analysis | Domain: Data Analysis

---

## 📝 Project Overview

This project focuses on predicting the likelihood of a person having diabetes based on various medical features such as glucose level, BMI, insulin, and age. It uses a structured machine learning pipeline to train, evaluate, and explain predictive models.

---

## 🔍 Dataset: `Diabetes.csv`
- **Records**: 768
- **Features**: Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age
- **Target**: Outcome (1 = Diabetic, 0 = Non-Diabetic)

---

## 🛠️ Workflow Summary

1. **Data Cleaning**
   - Replaced 0 values in key medical columns (e.g., Glucose, BMI) with median values
2. **Feature Engineering**
   - Added `Glucose_BMI` (interaction feature)
   - Binned `Age` into categorical groups (`Age_Group`)
3. **Data Preparation**
   - Scaled features using StandardScaler
   - Split data into training and testing sets
4. **Model Training**
   - Logistic Regression
   - Random Forest
   - Support Vector Machine (SVM)
5. **Evaluation**
   - Accuracy, Precision, Recall, F1-score
   - Confusion Matrix and Classification Report

---

## 📊 Model Results

| Model                 | Accuracy |
|-----------------------|----------|
| ✅ Logistic Regression | **76.6%** |
| Random Forest         | ~76%     |
| Support Vector Machine (SVM) | ~76%     |

![Image](https://github.com/user-attachments/assets/2a45ab57-b616-474d-9009-f5b52145746f)

---

## 📉 Why Accuracy Was Not Higher

- **Small Dataset**: Only 768 rows
- **Limited Features**: No lifestyle, dietary, or hereditary data included
- **Class Imbalance**: More non-diabetic cases than diabetic
- **Natural Uncertainty**: Some borderline patients cause ambiguity

> Despite these challenges, the model captures meaningful health patterns and offers a strong foundation for predictive analysis.

---

## 📦 Tools Used
**Python**, **VS Code**, **Pandas**, **Scikit-learn**, **Matplotlib**, **Seaborn**

---

## ✅ Conclusion

This project demonstrates a complete and realistic end-to-end machine learning workflow, including data preparation, model comparison, and evaluation. The methodology reflects best practices in healthcare prediction modeling.

