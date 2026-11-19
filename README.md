# Loan Approval Prediction

## Overview
A machine learning project that predicts whether a loan application
will be approved, based on applicant details such as income, credit
history, loan amount and property area.

## Dataset
Kaggle Loan Prediction dataset: 614 applications, 13 columns.

## Approach
1. Handled missing values (mode for categorical, median for numeric)
2. Engineered features: monthly installment (EMI), total income,
   log-transformed income columns, binary and one-hot encodings
3. Split data 80/20 (stratified) and standardized features
4. Trained and compared three classifiers
5. Evaluated with accuracy, precision, recall, F1 and confusion matrices

## Results
| Model         | Accuracy | Precision | Recall | F1     |
|---------------|----------|-----------|--------|--------|
| Decision Tree | 82.1%    | 0.825     | 0.941  | 0.879  |
| Naive Bayes   | 84.6%    | 0.830     | 0.976  | 0.897  |
| KNN           | 82.1%    | 0.800     | 0.988  | 0.884  |

Best model: Naive Bayes with 84.6% accuracy.

## Limitations
The models catch most approved loans but miss many rejected ones
(recall for rejections is about 55%). Future work: class balancing,
cross-validation, and trying Random Forest or Logistic Regression.

## Libraries
Python, pandas, NumPy, scikit-learn, matplotlib

## Author
Sohaima Said
