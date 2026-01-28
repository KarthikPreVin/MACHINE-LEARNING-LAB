# Machine Learning Laboratory - Assignment 2

## Objective

This repository contains the implementation and analysis for **Experiment #2: Binary Classification using Naive Bayes and K-Nearest Neighbors**. The objective of this assignment is to implement and evaluate Naive Bayes and KNN classifiers on a binary classification problem (Spambase dataset), analyzing their performance through various metrics and diagnostic visualizations.

## Author

* **Name:** Karthik. V
* **Reg No:** 3122235001064

## Tasks

* Implement **Naïve Bayes** (Gaussian, Multinomial, and Bernoulli variants) and **K-Nearest Neighbors (KNN)** classifiers.
* Evaluate model behavior using performance metrics including Accuracy, Precision, Recall, F1-score, and ROC-AUC.
* Visualize model performance using **Confusion Matrices** and **ROC Curves**.
* Analyze the **bias-variance trade-off** and the impact of hyperparameter tuning (e.g.,  value in KNN).
* Compare computational efficiency using different neighbor search methods such as **KDTree** and **BallTree**.


## Methodology

1. **Exploratory Data Analysis (EDA):** Visualization of class distribution and feature correlation using heatmaps to verify the independence assumption for Naive Bayes.
2. **Preprocessing:** Feature scaling using `MinMaxScaler` to normalize data between 0 and 1, ensuring distance-based algorithms like KNN perform accurately.
3. **Model Training & Tuning:**
* Training multiple Naive Bayes variants.
* Using `GridSearchCV` and `RandomizedSearchCV` to find optimal hyperparameters for KNN (Metric: Manhattan, Weights: Distance, ).
4. **Evaluation:** Comparison of training time, prediction time, and standard classification metrics across all models.

## Key Findings

* **Naive Bayes:** Performed well as feature correlation was not excessively high, satisfying the algorithm's independence assumption.
* **KNN:** Accuracy generally declined as  increased. An optimal  was selected to avoid high variance found at very low  values and high bias at very large  values.
* **Search Algorithms:** While KDTree and BallTree resulted in identical accuracy, they offered different efficiencies in terms of prediction time and memory usage.


## Files in this Repository

* `ASSIGNMENT 2.ipynb`: Jupyter Notebook containing the full Python implementation, including data loading, scaling, model training, and visualization code.
* `datasets`: 
    - [Spambase](datasets/dataset2.csv)


## Dependencies

* `pandas` (Data manipulation)
* `scikit-learn` (ML algorithms, preprocessing, and metrics)
* `matplotlib` & `seaborn` (Visualization)
* `time` (Computational profiling)

---