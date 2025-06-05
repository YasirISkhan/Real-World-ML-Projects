
# 💻 Laptop Price Prediction using Machine Learning

## 📌 Project Overview

This project aims to predict the price of a laptop based on various features such as brand, RAM, storage, processor type, GPU, screen resolution, etc. The objective is to build a regression model that accurately estimates the price of a laptop using machine learning techniques.

The final deployed model uses **RandomForestRegressor**, which achieved the **highest R² score** and **lowest Mean Absolute Error (MAE)** among all evaluated models.

---

## 📊 Dataset

The dataset was scraped from various e-commerce platforms and cleaned before modeling. It contains the following features:

- Brand / Company
- Model Name
- RAM (in GB)
- Storage (HDD, SSD, etc.)
- Processor type
- GPU (Graphics Card)
- Operating System
- Screen Size
- Screen Resolution
- Touchscreen or not
- IPS Panel or not
- Weight
- Price (Target Variable)

---

### 2. Model Training

Tested the following regression algorithms:

| Algorithm              | R2 Score & MAE |
|------------------------|-------------|
| Linear Regression      | 78% & 21    |
| Ridge Regression       |  79% & 21   |
| Lasso Regression       | 78% & 21    |
| KNN                    | 80% & 0.19  |
| Decision Tree          | 84% & 0.18  |
| Gradient Boosting      | 88% & 0.15  |
| XGBoost Regressor      | 89% & 0.15  |
| Stacking               | 88% & 0.16  |
| Voting Regressor       | 89% & 0.15  |
| **Random Forest**      | ✅ **90 & 0.14**  |

## 🛠️ Technologies Used

- Python
- Jupyter Notebook / PyCharm
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Flask (for web deployment)
- Git & GitHub

---

## 📈 Machine Learning Workflow

### 1. Data Preprocessing
- Handled missing values and outliers.
- Converted categorical columns using encoding.
- Extracted numeric resolution from screen details.
- Combined memory components into structured features (HDD, SSD, etc.).
- Converted "yes"/"no" fields into binary format.

### 3. Hyperparameter Tuning

Used **GridSearchCV** to optimize hyperparameters for `RandomForestRegressor`, such as:

- `n_estimators`
- `random_state`
- `max_samples`
- `max_features`
- `max_depth`

---

## ✅ Final Model

- **Algorithm**: RandomForestRegressor
- **R² Score**: *Highest among all models*
- **MAE (Mean Absolute Error)**: *Lowest*
- **Hyperparameter Optimization**: GridSearchCV

---



## 📷 Screenshot
![Structure of Project](https://github.com/YasirISkhan/Real-World-ML-Projects/blob/eb104f3692e29ec02c5fa8146b5a3265806a0a5a/Laptop%20Price%20Predictor/Images/Application%20Options.jpg)

![Structure of Project](https://github.com/YasirISkhan/Real-World-ML-Projects/blob/eb104f3692e29ec02c5fa8146b5a3265806a0a5a/Laptop%20Price%20Predictor/Images/Screenshot%202025-06-05%20123328.png)
