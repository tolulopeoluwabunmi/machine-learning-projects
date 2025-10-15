# 🌸 Iris Classification (KNN, Naive Bayes, Logistic Regression)

**Goal:** Predict the species of Iris flowers using sepal and petal measurements.

## 🧩 Dataset Overview
- 150 samples, 4 numerical features, 3 classes (Setosa, Versicolor, Virginica)
- Perfectly balanced dataset - no missing values
- Source: Kaggle

## ⚙️ Models Used
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes
- Logistic Regression

## 📊 Results
| Model | Accuracy | Notes |
|--------|-----------|-------|
| Logistic Regression | 96.7% | Smooth decision boundaries |
| GaussianNB | 96.7% | Excellent baseline model |
| KNN | 95% | Slight overlap between Versicolor & Virginica |

✅ **Best Model:** Logistic Regression & GaussianNB (tie at 96.7%)

## 🧮 Techniques
- Data scaling with `StandardScaler`
- Train–test split (60/40 stratified)
- Performance metrics: Accuracy, Confusion Matrix, F1-score

## 📁 Files in this Folder
- `Iris_Classification.ipynb` — runnable Jupyter notebook  
- `Iris_Classification_Report.pdf` — detailed report with visuals and explanations

