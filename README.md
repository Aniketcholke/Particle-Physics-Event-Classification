# Particle-Physics-Event-Classification
Overview

This project focuses on classifying data into target labels using machine learning models while performing exploratory data analysis (EDA) and feature importance analysis. The goal is to build robust predictive models and derive insights into the most influential features.

Project Objective

1) Build predictive models to classify events into target labels.
2) Identify and rank key features that contribute to predictions.
3) Ensure data preprocessing and analysis adhere to best practices.

Project Workflow

1. Data Preprocessing
   
Loaded the dataset using Pandas.
Inspected the dataset structure using .info(), .describe(), and .head().
Handled missing values, duplicates, and outliers using:
Interquartile Range (IQR): Detected and capped extreme values.
Ensured all features were clean and ready for analysis.

2. Exploratory Data Analysis (EDA)

Boxplots: Visualized numerical feature distributions and outliers.
Correlation Heatmap: Explored relationships between features.
Class Distribution: Checked for class imbalance and determined that no additional treatment was necessary.

3. Feature Engineering

Dropped irrelevant columns (e.g., EventId).
Identified the top 10 most important features using Random Forest’s feature importance scores.

4. Model Building

Implemented the following models:
Logistic Regression: A baseline model for classification.
Random Forest: An ensemble model for capturing complex relationships.
Evaluated models using:
Accuracy, Precision, Recall, F1-Score.
Confusion Matrix.
ROC-AUC for Logistic Regression.

5. Cross-Validation

Used 10-fold cross-validation to validate model consistency and prevent overfitting.
Reported metrics like average accuracy and maximum accuracy.
