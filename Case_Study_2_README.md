# Case Study 2: Credit Card Fraud Detection

## Objective

The objective of this case study is to detect fraudulent credit card transactions using machine learning.

## Dataset

The Credit Card Fraud Detection dataset contains 284,807 transactions, including 492 fraudulent transactions. The dataset is highly imbalanced.

## Machine Learning Model

XGBoost Classifier was used for fraud detection.

## Imbalance Handling

SMOTE (Synthetic Minority Over-sampling Technique) was applied only to the training data to address class imbalance.

## Methodology

1. Load and inspect the dataset
2. Check class distribution
3. Check missing values
4. Separate features and target
5. Split the dataset into training and testing sets
6. Apply SMOTE to the training data
7. Train the XGBoost model
8. Generate fraud probabilities
9. Evaluate using ROC-AUC
10. Tune the decision threshold
11. ## Results

- Model: XGBoost
- Imbalance Handling: SMOTE
- ROC-AUC: 0.9785
- Selected Threshold: 0.50
- Precision: 0.7265
- Recall: 0.8673
- F1-Score: 0.7907

## Confusion Matrix

- True Negatives (TN): 56832
- False Positives (FP): 32
- False Negatives (FN): 13
- True Positives (TP): 85

## Feature Importance

The most important feature according to the XGBoost model was V14.
12. Analyze feature importance
## Results

- Model: XGBoost
- Imbalance Handling: SMOTE
- ROC-AUC: 0.9785
- Selected Threshold: 0.50
- Precision: 0.7265
- Recall: 0.8673
- F1-Score: 0.7907

## Confusion Matrix

- True Negatives (TN): 56832
- False Positives (FP): 32
- False Negatives (FN): 13
- True Positives (TP): 85

## Feature Importance

The most important feature according to the XGBoost model was V14.
