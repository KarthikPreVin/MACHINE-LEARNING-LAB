# Machine Learning Laboratory - Assignment 3

## Objective

This repository contains the implementation **Experiment #3: Regression Analysis using Linear and Regularized Models**. The project focuses on predicting a continuous target variable (Loan Sanction Amount) by implementing standard linear regression, regularized linear regression and Support Vector Regression.

## Author

* **Name:** Karthik. V
* **Reg No:** 3122235001064

## Tasks

* Implement **Linear Regression** and its regularized variants: **Ridge**, **Lasso**, and **Elastic Net**.
* Explore non-linear regression using **Support Vector Regression (SVR)** with different kernels.
* Perform rigorous data preprocessing including imputation of missing values and encoding of categorical variables.
* Evaluate models using comprehensive regression metrics: **MAE**, **MSE**, **RMSE**, , and **Adjusted **.
* Analyze the impact of regularization on the bias-variance trade-off.

## Dataset Description

The analysis is performed on a **Loan Dataset** (30,000 entries) with the following characteristics:

* **Target Variable:** `Loan Sanction Amount (USD)`
* **Key Features:** Income, Age, Income Stability, Profession, Type of Employment, and Credit Score.
* **Challenges:** Missing values in features like `Gender`, `Income`, and `Credit Score`.

## Methodology

1. **Data Preprocessing:**
* **Handling Missing Values:** Used `SimpleImputer` with 'median' for numerical data and 'most_frequent' for categorical data.
* **Encoding:** Transformed categorical labels into numerical formats using `OrdinalEncoder`.
* **Scaling:** Applied `StandardScaler` to ensure all features contribute equally to the distance-based SVR model.

2. **Modeling Techniques:**
* **Ordinary Least Squares (OLS):** Standard Linear Regression.
* **Regularization:** Comparison of  (Lasso),  (Ridge), and combined (Elastic Net) penalties.
* **SVR Tuning:** Hyperparameter optimization for the Support Vector Regressor.

3. **Cross-Validation:** Implemented **K-Fold Cross-Validation** () to ensure the robustness of the performance metrics.

## Performance Summary

| Model | MAE | MSE | RMSE |  Score |
| --- | --- | --- | --- | --- |
| **Linear Regression** | 0.3152 | 0.1570 | 0.3963 | 0.7012 |
| **Ridge Regression** | 0.3152 | 0.1570 | 0.3963 | 0.7012 |
| **Lasso Regression** | 0.3151 | 0.1571 | 0.3963 | 0.7011 |
| **SVR** | 0.3560 | 0.1982 | 0.4452 | 0.6226 |

## Files in this Repository

* `ASSIGNMENT 3.ipynb`: Jupyter Notebook containing code for imputation, feature scaling, model training, and metric calculation.
* `datasets`: 
    - [Training Data (Loan Amount Prediction)](datasets/dataset3_train.csv)
    - [Testing Data (Loan Amount Prediction)](datasets/dataset3_test.csv)

## Dependencies

* `pandas` (Data manipulation)
* `scikit-learn` (ML algorithms, preprocessing, and metrics)
* `matplotlib` & `seaborn` (Visualization)
* `time` (Computational profiling)
---
