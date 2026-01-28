# Machine Learning Laboratory - Assignment 4

## Overview

This repository contains the work for **Experiment #4: Binary Classification using Linear and Kernel-Based Models**. The assignment focuses on the classification of emails as spam using **Logistic Regression** and **Support Vector Machines (SVM)**. The primary objective of this experiment is to analyze the impact of different SVM kernels and hyperparameter tuning on overall classification performance.

## Author

* **Name:** Karthik. V
* **Reg No:** 3122235001064

## Objectives

* Implement a binary classifier for the **Spambase dataset**.
* Optimize **Logistic Regression** using `GridSearchCV` (tuning , penalty, and solvers).
* Compare the performance of various **SVM Kernels**: Linear, Polynomial, RBF, and Sigmoid.
* Evaluate models using performance metrics: Accuracy, Precision, Recall, and F1-score.
* Conduct a **K-Fold Cross-Validation** (5 fold) to assess model stability and generalization.

## Key features and Methodology

1. **Data Preprocessing:**
* **Feature Scaling:** Applied `StandardScaler` to normalize the 57 continuous features, which is critical for the distance-based SVM algorithm.

2. **Model Training:**
* **Baseling Model**
* **Logistic Regression Tuning:** 
* **SVM Tuning:** 

3. **Cross-Validation:** Used 5-Fold CV to mitigate overfitting and ensure consistent accuracy across different subsets of the data.

## Performance Comparison

The following results were obtained on the test set after hyperparameter tuning:

### Model Performance Summary

| Metric | Logistic Regression | Best SVM (RBF) |
| --- | --- | --- |
| **Accuracy** | 0.9414 | 0.9359 |
| **Precision** | 0.9399 | 0.9526 |
| **Recall** | 0.9149 | 0.8872 |
| **F1 Score** | 0.9272 | 0.9188 |
| **Training Time** | 1.7 ms | 122.2 ms |

### SVM Kernel-wise Comparison

| Kernel | Accuracy | F1 Score | Training Time (ms) |
| --- | --- | --- | --- |
| **Linear** | 0.9435 | 0.9295 | 23.9 |
| **Polynomial** | 0.9283 | 0.9088 | 45.0 |
| **RBF** | 0.9359 | 0.9195 | 122.2 |
| **Sigmoid** | 0.9001 | 0.8757 | 48.0 |

## Files in this Repository

* `ASSIGNMENT 4.ipynb`: Jupyter Notebook containing the full pipeline: data scaling, `GridSearchCV` implementations, kernel comparisons, and evaluation plots.
* `datasets`: 
    - [Spambase](datasets/dataset4.csv)

## Dependencies

* `pandas` (Data manipulation)
* `scikit-learn` (ML algorithms, preprocessing, and metrics)
* `matplotlib` & `seaborn` (Visualization)
* `time` (Computational profiling)

---