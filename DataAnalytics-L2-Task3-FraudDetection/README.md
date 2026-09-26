# 💳 Credit Card Fraud Detection

A machine learning project for detecting fraudulent credit card transactions using Python and Scikit-learn.

## 📌 Project Overview

Credit card fraud detection is a highly imbalanced classification problem where fraudulent transactions represent only a very small portion of all transactions.

This project explores the dataset, handles class imbalance using SMOTE, trains multiple machine learning models, and evaluates them using fraud-detection-focused metrics such as Precision, Recall, F1-Score, and ROC-AUC.

## 🎯 Objectives

- Explore and understand the credit card transaction dataset
- Analyze class imbalance and fraudulent transaction patterns
- Identify time-based fraud patterns
- Remove duplicate records
- Handle class imbalance using SMOTE
- Train Logistic Regression and Random Forest models
- Compare model performance using appropriate evaluation metrics
- Analyze important features influencing fraud predictions
- Discuss scalability for high-volume transaction processing

## 📊 Dataset

The project uses the Credit Card Fraud Detection dataset.

The dataset contains:

- 284,807 transactions
- 31 original columns
- 492 fraudulent transactions
- 284,315 legitimate transactions

After duplicate removal:

- 283,726 transactions
- 473 fraudulent transactions
- 283,253 legitimate transactions

Fraudulent transactions represented approximately **0.17%** of the cleaned dataset.

> The dataset is not included in this repository because the CSV file is too large for GitHub's standard file-size limit.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- Jupyter Notebook

## 🔍 Project Workflow

```text
Data Loading
     ↓
Data Inspection
     ↓
Missing Value Analysis
     ↓
Duplicate Detection & Removal
     ↓
Exploratory Data Analysis
     ↓
Time-of-Day Analysis
     ↓
Correlation Analysis
     ↓
Train-Test Split
     ↓
SMOTE on Training Data
     ↓
Feature Scaling
     ↓
Model Training
     ├── Logistic Regression
     └── Random Forest
     ↓
Model Evaluation
     ↓
Feature Importance Analysis
     ↓
Final Comparison

## 📈 Model Performance

### Logistic Regression

- Precision: 0.1406
- Recall: 0.8526
- F1-Score: 0.2414
- ROC-AUC: 0.9646

### Random Forest

- Precision: 0.9012
- Recall: 0.7684
- F1-Score: 0.8295
- ROC-AUC: 0.9507

### Model Comparison

|        Model        | Precision | Recall | F1-Score | ROC-AUC |
|---------------------|----------:|-------:|---------:|--------:|
| Logistic Regression |   0.1406  | 0.8526 |  0.2414  |  0.9646 |
|    Random Forest    |   0.9012  | 0.7684 |  0.8295  |  0.9507 |

The models demonstrate a precision-recall trade-off. Logistic Regression detected a larger proportion of fraudulent transactions, while Random Forest produced substantially fewer false-positive fraud predictions.

