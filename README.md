# credit-card-fraud-detection-ml
# Credit Card Fraud Detection using Machine Learning

## Overview
This project builds a machine learning system to detect fraudulent credit card transactions using behavioral transaction data.

The dataset includes features such as:
- Distance from home
- Distance from last transaction
- Ratio to median purchase price
- Online transaction indicator

The goal is to classify transactions as fraudulent or legitimate transactions using supervised machine learning models.

---

## Problem Statement
Credit card fraud detection is a highly imbalanced classification problem where fraudulent transactions are rare compared to legitimate ones. Traditional accuracy is not a reliable metric, so this project focuses on precision, recall, and F1-score to properly evaluate model performance.

---

## Dataset
The dataset contains transaction-level data with features representing customer behavior and transaction patterns. The target variable indicates whether a transaction is fraudulent (1) or legitimate (0).

Key characteristics:
- Large dataset size
- Highly imbalanced classes
- Behavioral and distance-based features

---

## Project Structure

```
credit-card-fraud-detection-ml/
│
├── data/
│   ├── raw/              # Original dataset (not modified)
│   └── processed/        # Cleaned dataset
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda.ipynb
│   └── 03_modeling.ipynb
│
├── src/
│   ├── preprocess.py     # Data loading and cleaning
│   ├── features.py       # Feature engineering
│   ├── train.py          # Model training
│   └── evaluate.py       # Model evaluation
│
├── outputs/
│   ├── figures/          # Graphs and visualizations
│   └── metrics/          # Model performance results
│
├── requirements.txt
└── README.md
```

---

## Models Used
- Logistic Regression
- Random Forest
- XGBoost (optional)

---

## Evaluation Metrics
Because the dataset is imbalanced, the following metrics are used:

- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

---

## Workflow

1. Data Loading
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Model Training
6. Model Evaluation
7. Results Visualization

---

## How to Run

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Run training pipeline
```bash
python src/train.py
```

---

## Notes
- The dataset is highly imbalanced, so special techniques like class weighting or resampling may be used.
- Feature engineering is important for improving model performance.
- The focus is on detecting fraud effectively rather than maximizing accuracy.

---

## Future Improvements
- Hyperparameter tuning
- Advanced models (XGBoost, Neural Networks)
- Real-time fraud detection system
- Deployment as a web application

---

## Author
Anirudh Iyer
