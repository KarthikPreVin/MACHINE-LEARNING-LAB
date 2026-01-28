# Machine Learning Laboratory - Assignment 1

## Objective

This repository contains the work for **Experiment #1: Working with Python packages - Numpy, Scipy, Scikit-Learn, Matplotlib**. The objective of this assignment is to perform Exploratory Data Analysis (EDA), data preprocessing, and feature selection on specific datasets to understand data relationships and prepare them for machine learning workflows.

## Author

* **Name:** Karthik. V
* **Reg No:** 3122235001064

## Tasks

* Perform array manipulations and mathematical computing using **NumPy**.
* Implement data preprocessing and analysis using **Pandas**.
* Visualize data distributions and relationships using **Matplotlib** and **Seaborn**.
* Execute feature selection tasks using ANOVA and Chi-squared tests via **Scikit-Learn**.

## Key Features & Methodology

1. **Data Exploration:** * Distribution analysis using bar graphs and histograms.
* Outlier detection and statistical inference (Median, IQR) through Box Plots.
* Linear relationship visualization via Correlation Heatmaps.


2. **Preprocessing:**
* **Encoding:** Categorical variables converted using `LabelEncoder`.
* **Imputation:** Handling missing values through Median and Mode imputation techniques.
* **Scaling:** Data centralization using Standard Scaling (mean=0, variance=1).


3. **Feature Selection:**
* **ANOVA (F-test):** Used for numerical feature significance.
* **Chi-Squared Test:** Used to determine independence between categorical variables.



## Datasets Used

* **Iris Dataset:** Analysis of sepal and petal dimensions for species classification.
* **Loan Dataset:** Analysis of loan applicant data (Income, Credit History, etc.) for predicting loan status.
* **Diabetes Dataset:** Analysis of person data for predicting future risk of diabetes.
* **Spambase Dataset:** Analysis of email words for classifying as spam.
* **Handwritten Digits Dataset:** Analysis of preprocessed Handwritten numbers for a multiclass classification problem. 

## Files in this Repository

* `ASSIGNMENT 1.ipynb`: The primary Jupyter Notebook containing Python code, data visualizations (histograms, bar charts, heatmaps), and statistical test implementations.
* `datasets`:
    - [Diabetes](datasets/dataset1_Diabetes.csv)
    - [Iris](datasets/dataset1_Iris.csv)
    - [Loan Classification](datasets/dataset1_Loan.csv)
    - [Handwritten Digits](datasets/dataset1_Numbers.csv)
    - [Spambase](datasets/dataset1_Spammail.csv)

## Dependencies

The following Python libraries are required to run the notebook:

* `pandas`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `numpy`

---