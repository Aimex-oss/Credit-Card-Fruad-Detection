# Notebook Details

# Credit Card Fraud Detector
This repository contains a Jupyter notebook that demonstrates a machine learning approach to detect fraudulent credit card transactions. The project is designed to tackle the challenge of identifying fraudulent transactions within a highly imbalanced dataset.

## Dataset Overview
The dataset includes credit card transactions made by European cardholders in **September 2013** over a period of **two days**. The dataset is notable for its **class imbalance**, with only **492 fraudulent transactions** out of **284,807 total transactions**, meaning frauds represent only **0.172%** of all transactions.

### Key Characteristics:
- **Number of Transactions**: 284,807
- **Number of Fraudulent Transactions**: 492
- **Time Period**: Two days
- **Class Imbalance**: Fraudulent transactions account for only 0.172% of all transactions.

## Features and Labels
The dataset consists entirely of **numerical input variables**, transformed through **Principal Component Analysis (PCA)**, except for the `Time` and `Amount` features. Due to confidentiality, the original features and background information are not available.

### **Features:**
- **V1 to V28**: Principal components derived from PCA.
- **Time**: The elapsed time in seconds between each transaction and the first transaction in the dataset.
- **Amount**: The monetary value of the transaction. It can be used for cost-sensitive learning models.

### **Label:**
- **Class**: 
  - `0`: Non-fraudulent transaction (Normal)
  - `1`: Fraudulent transaction (Fraud)

### **Class Distribution:**
- **Non-Fraudulent (Class 0)**: Majority of the dataset
- **Fraudulent (Class 1)**: Only 0.172% of the dataset

## Objective
The primary goal is to build a model that can accurately detect fraudulent transactions despite the severe class imbalance. The **Area Under the Precision-Recall Curve (AUPRC)** is recommended as the primary evaluation metric, as traditional accuracy metrics can be misleading in such unbalanced scenarios.

## Key Features of the Project:
- **Data Preprocessing**: Handling missing values, normalization, and balancing techniques.
- **Modeling**: Training various machine learning models including logistic regression, decision trees, random forests, and gradient boosting.
- **Evaluation**: Emphasis on AUPRC for model evaluation due to class imbalance.

## Dataset can be donwloaded from 
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data

## How to Use
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detector.git
   cd credit-card-fraud-detector

