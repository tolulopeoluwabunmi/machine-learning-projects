### Spam Email Classification (KNN, Logistic Regression, PCA)

Goal: Predict whether an email is spam based on its textual and structural features such as word frequency, character usage, and capitalization patterns.

📊 Dataset Overview

Source: Kaggle – Spambase Dataset

Records: 4,601 emails

Features: 57 numerical attributes + 1 target column

Target: 0 = Non-Spam, 1 = Spam

Balance: 61% non-spam vs 39% spam (slightly imbalanced)

Missing Values: None

⚙️ Preprocessing

Scaled features using StandardScaler.

Applied Principal Component Analysis (PCA) → 35 components explaining 81% variance.

Stratified 60/40 train-test split to maintain class proportions.

🧪 Models Tested
Model	Test Accuracy	Mean CV Accuracy	RMSE	Key Notes
Logistic Regression	0.910	0.887	0.300	Strong baseline, interpretable
KNN (tuned, k = 15, weights = ‘distance’)	0.920	0.899	0.284	Best accuracy and precision
📈 Insights

Both models achieved over 90% accuracy.

KNN performed slightly better and captured complex nonlinear relationships.

PCA reduced dimensionality while retaining essential information.

The results were consistent across 5-fold cross-validation.

🧩 Key Steps

Data loading and exploration

Standardization and PCA

Model training and tuning

Evaluation (confusion matrix, classification report, cross-validation)

📂 Files

Spambase.ipynb – Main notebook with preprocessing, PCA, and modeling.

Spambase.pdf – Final project report with visuals and evaluation results.

README.md – Project summary and insights.
