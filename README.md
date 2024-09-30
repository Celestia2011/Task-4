# Task-4: Heart Disease Prediction using Random Forest

This project implements a Random Forest algorithm to predict heart disease based on a medical dataset containing various health attributes. The analysis compares the performance of the model with and without data normalization, with a focus on accuracy and other evaluation metrics.
Introduction

This project aims to develop a machine learning model using the Random Forest algorithm for predicting heart disease. We explore the effect of data normalization on model performance and evaluate key metrics such as accuracy and confusion matrices for both normalized and non-normalized datasets.
Dataset

The dataset contains various attributes related to heart disease, such as:

    Age
    Sex
    Chest Pain Type
    Resting Blood Pressure
    Cholesterol
    Max Heart Rate
    Exercise-Induced Angina
    ST Depression
    Heart Disease (Target variable)

Methodology

The project follows these key steps:

    Data Preprocessing: The dataset is split into training and testing sets. We perform normalization for Task B, while Task A uses raw data.
    Random Forest Model: A Random Forest classifier is implemented to predict heart disease. The model's hyperparameters are optimized using grid search with cross-validation.
    Evaluation: Model performance is evaluated using accuracy, confusion matrices, and hyperparameter tuning results.

Task A: Analysis without Normalization

    Initial model accuracy: 0.8641
    Best hyperparameters:
        max_depth: 10
        min_samples_leaf: 1
        min_samples_split: 2
        n_estimators: 200
    Best model accuracy: 0.8859

Task B: Analysis with Normalization

    Initial model accuracy: 0.8750
    Best hyperparameters:
        max_depth: 10
        min_samples_leaf: 1
        min_samples_split: 2
        n_estimators: 300
    Best model accuracy: 0.8913

## Results Comparison

| Metric                  | Non-normalized | Normalized   |
|-------------------------|----------------|--------------|
| Initial Accuracy         | 0.8641         | 0.8750       |
| Best Model Accuracy      | 0.8859         | 0.8913       |
| Best Parameters          | `max_depth: 10, min_samples_leaf: 1, min_samples_split: 2, n_estimators: 200` | `max_depth: 10, min_samples_leaf: 1, min_samples_split: 2, n_estimators: 300` |


Normalization slightly improved the model's performance, especially after hyperparameter tuning.
