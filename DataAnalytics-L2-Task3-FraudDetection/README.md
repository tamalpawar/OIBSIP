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
```
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

## 🔬 Feature Importance Analysis

Random Forest feature importance was used to identify the features that contributed most strongly to the model's predictions.

### Top 15 Features

| Feature | Importance |
|---|---:|
| V14 | 0.229394 |
| V10 | 0.164196 |
| V12 | 0.108078 |
| V4 | 0.088294 |
| V11 | 0.071929 |
| V17 | 0.071911 |
| V3 | 0.060649 |
| V16 | 0.028076 |
| V7 | 0.027145 |
| V2 | 0.023990 |
| V9 | 0.023407 |
| V21 | 0.013735 |
| V18 | 0.012696 |
| V1 | 0.007527 |
| V6 | 0.007073 |

The notebook also includes Logistic Regression coefficient analysis to examine the direction and relative influence of features.

## ⚖️ Class Imbalance Handling

The dataset contains a very small proportion of fraudulent transactions.

SMOTE (Synthetic Minority Oversampling Technique) was applied **only to the training data** to address class imbalance while keeping the test set unchanged.

### Before SMOTE

| Class | Samples |
|---|---:|
| 0 - Legitimate | 226,602 |
| 1 - Fraud | 378 |

### After SMOTE

| Class | Samples |
|---|---:|
| 0 - Legitimate | 226,602 |
| 1 - Fraud | 226,602 |

The test set remained untouched for final model evaluation.

## 📊 Evaluation Metrics

The models were evaluated using:

- **Precision** – proportion of transactions predicted as fraud that were actually fraudulent
- **Recall** – proportion of actual fraudulent transactions detected by the model
- **F1-Score** – harmonic mean of precision and recall
- **ROC-AUC** – measures the model's ability to distinguish between fraudulent and legitimate transactions

Because the dataset is highly imbalanced, accuracy alone was not used as the primary evaluation metric.

## 📈 Key Visualizations

The `outputs/` folder contains the main analysis visualizations:

- Fraud rate by hour
- Logistic Regression coefficients
- Random Forest feature importance
- ROC-AUC model comparison
- Top feature correlations

## 📁 Project Structure

```text
DataAnalytics-L2-Task3-FraudDetection/
│
├── Fraud_Detection.ipynb
├── README.md
├── .gitignore
│
└── outputs/
    ├── fraud_rate_by_hour.png
    ├── logistic_regression_coefficients.png
    ├── random_forest_feature_importance.png
    ├── roc_auc_comparison.png
    └── top_features_correlation.png
```

## 🚀 Future Improvements

- Hyperparameter tuning
- Threshold optimization for fraud detection
- Precision-Recall curve analysis
- Cross-validation
- Testing additional ensemble models
- Model deployment as an API
- Real-time fraud detection pipeline
- Monitoring model performance on new transaction data

## 👨‍💻 Author

**Tamalkrishna Pawar**

