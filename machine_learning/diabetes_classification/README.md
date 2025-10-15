### Diabetes Classification (Logistic Regression, KNN, Decision Tree, PCA)

Goal: Predict whether a patient has diabetes using diagnostic measurements such as glucose level, BMI, and age.

📊 Dataset Overview

Source: Kaggle – Pima Indians Diabetes Dataset

Records: 768 patients

Features: 8 numeric predictors

Target: Binary outcome (0 = non-diabetic, 1 = diabetic)

⚙️ Data Cleaning

Replaced physiologically impossible zero values in Glucose, BMI, BloodPressure, SkinThickness, and Insulin with column medians.

Standardized all features using StandardScaler.

Applied Principal Component Analysis (PCA) to reduce redundancy — top 3 components explained ~90% of the variance.

🧪 Models Tested
Model	Accuracy	Key Notes
Logistic Regression	75%	Best generalization and interpretability
K-Nearest Neighbors (KNN)	73%	Good accuracy, sensitive to scaling
Decision Tree	69%	Slightly overfits, lower stability
Logistic Regression (PCA)	73%	Simpler model, minimal accuracy loss
📈 Results Summary

Logistic Regression performed best overall.

PCA achieved dimensionality reduction without significant information loss.

Cross-validation confirmed model consistency (mean accuracy ≈ 77%).

Glucose, BMI, and Age were the top predictors.

🧩 Key Insights

High glucose and BMI levels are strong indicators of diabetes.

PCA improved computational efficiency and interpretability.

The workflow is clean, reproducible, and ready for unseen data validation.

📂 Files

Diabetes.ipynb: Notebook with EDA, modeling, and evaluation.

Diabetes_Report.pdf: Full written report with visuals and explanations.

README.md: Summary of methodology and key insights.
