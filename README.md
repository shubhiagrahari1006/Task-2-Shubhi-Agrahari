# Credit Card Fraud Detection Using Machine Learning

## Project Overview

This project focuses on detecting fraudulent credit card transactions using Machine Learning techniques. The primary challenge in fraud detection is the highly imbalanced nature of the dataset, where fraudulent transactions represent only a tiny fraction of total transactions.

To address this challenge, data preprocessing, class balancing using SMOTE (Synthetic Minority Oversampling Technique), and supervised machine learning models were implemented and evaluated.

The project demonstrates a complete end-to-end fraud detection workflow, including data exploration, preprocessing, imbalance handling, model training, evaluation, and performance comparison.

---

## Problem Statement

Credit card fraud causes significant financial losses worldwide. Traditional machine learning models often struggle with such datasets because fraudulent transactions are extremely rare compared to legitimate transactions.

The objective of this project is to build and evaluate classification models capable of accurately identifying fraudulent transactions while minimizing false predictions.

---

## Dataset Information

**Dataset:** Credit Card Fraud Detection Dataset

### Dataset Source

The dataset used in this project is publicly available on Kaggle:

https://www.kaggle.com/datasets/isaikumar/creditcardfraud

### Target Variable

| Class | Description |
|---------|------------|
| 0 | Legitimate Transaction |
| 1 | Fraudulent Transaction |

### Dataset Characteristics

- Highly Imbalanced Dataset
- Binary Classification Problem
- Real-world financial transaction data
- Suitable for fraud detection research and machine learning applications

---

## Project Workflow

### 1. Data Loading and Understanding

- Loaded dataset using Pandas
- Explored dataset structure and dimensions
- Examined data types and summary statistics

### 2. Data Quality Assessment

- Checked for missing values
- Checked for duplicate records
- Removed duplicate observations

### 3. Exploratory Data Analysis (EDA)

- Analyzed fraud and non-fraud transaction distribution
- Visualized class imbalance
- Identified the need for oversampling techniques

### 4. Handling Class Imbalance

Applied **SMOTE (Synthetic Minority Oversampling Technique)** to balance the minority class in the training dataset.

#### Before SMOTE

| Class | Count |
|---------|---------|
| Legitimate Transactions | 226,602 |
| Fraudulent Transactions | 378 |

#### After SMOTE

| Class | Count |
|---------|---------|
| Legitimate Transactions | 226,602 |
| Fraudulent Transactions | 226,602 |

---

## Machine Learning Models Implemented

### Logistic Regression

A baseline classification model used to establish initial fraud detection performance.

### Random Forest Classifier

An ensemble machine learning algorithm that combines multiple decision trees to improve predictive accuracy and robustness.

---

## Model Evaluation Metrics

The following evaluation metrics were used:

- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Confusion Matrix

Since fraud detection involves highly imbalanced classes, special emphasis was placed on Recall, F1-Score, and ROC-AUC rather than overall accuracy.

---

## Results

| Model | Precision | Recall | F1-Score | ROC-AUC |
|---------|---------|---------|---------|---------|
| Logistic Regression | 0.11 | 0.87 | 0.20 | 0.9536 |
| Random Forest | 0.89 | 0.77 | 0.82 | 0.9609 |

---

## Best Performing Model

### Random Forest Classifier

Random Forest achieved the strongest overall performance based on:

- Highest Precision
- Highest F1-Score
- Highest ROC-AUC Score
- Better balance between fraud detection and false alarms

Therefore, Random Forest was selected as the best-performing model for this fraud detection task.

---

## Technologies and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Imbalanced-Learn (SMOTE)
- Jupyter Notebook

---

## Repository Structure

```text
├── Project2_Fraud_Detection.ipynb
├── README.md
├── class_distribution.png
├── smote_before_after.png
└── model_comparison.png
```

---

## Key Learning Outcomes

- Data preprocessing and cleaning
- Exploratory Data Analysis (EDA)
- Handling highly imbalanced datasets
- SMOTE implementation
- Fraud detection using machine learning
- Logistic Regression modeling
- Random Forest modeling
- Model evaluation using advanced classification metrics
- Comparative performance analysis

---

## Screenshots

### Class Distribution
Shows the severe imbalance between legitimate and fraudulent transactions.

### SMOTE Balancing
Illustrates the class distribution before and after applying SMOTE.

### Model Comparison
Compares Logistic Regression and Random Forest based on Precision, Recall, F1-Score, and ROC-AUC.

---

