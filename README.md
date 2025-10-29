# Wine_Quality_Predictor
This project aims to predict the quality of red wine based on various physicochemical properties using different machine learning algorithms. The dataset used is the Wine Quality Dataset (Red Wine), which contains information about the chemical characteristics of wine samples and their corresponding quality scores.

# 🍷 Wine Quality Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Model-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-success)

## 📘 Project Overview
This project focuses on predicting the **quality of red wine** based on various physicochemical properties using **machine learning algorithms**.  
The main goal is to classify wine samples into quality categories and determine which features most strongly influence wine quality.

The dataset used is the **Wine Quality - Red Wine Dataset** from the UCI Machine Learning Repository.

---

## 📂 Dataset
- **File:** `winequality-red.csv`  
- **Description:** Contains 11 physicochemical features (such as acidity, sugar, and pH) and one quality score (ranging from 3 to 8).  

**Features include:**
- Fixed acidity  
- Volatile acidity  
- Citric acid  
- Residual sugar  
- Chlorides  
- Free sulfur dioxide  
- Total sulfur dioxide  
- Density  
- pH  
- Sulphates  
- Alcohol  
- **Target:** Quality (score between 0–10)

---

## ⚙️ Project Workflow

### 1️⃣ Data Preprocessing
- Load dataset using **Pandas**.
- Split data into features (`X`) and target (`Y`).
- Apply **StandardScaler** to normalize input features.
- Split into **training (80%)** and **testing (20%)** sets.

### 2️⃣ Model Training
Implemented and compared three different models:
- **Logistic Regression** (baseline)
- **Random Forest Classifier**
- **Decision Tree Classifier**

### 3️⃣ Model Evaluation
Used various metrics from **scikit-learn**:
- Accuracy Score  
- Classification Report (Precision, Recall, F1-score)  
- ROC AUC Score  

### 4️⃣ Model Saving
Saved the best-performing model (**Random Forest**) using:
```python
joblib.dump(rf, 'random_forest_model.pkl')

