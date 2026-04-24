# Confusion Matrix, Precision, Recall & F1-Score

This project explains how to evaluate classification models using **Confusion Matrix**, **Precision**, **Recall**, and **F1-Score** with Python and Scikit-learn.
It helps in understanding how well a classification model performs beyond just accuracy.

---

## 1. Confusion Matrix

A **Confusion Matrix** is a simple and useful tool used to measure the performance of a classification model.

It shows the number of:
- Correct Predictions
- Incorrect Predictions
- True Positives
- True Negatives
- False Positives
- False Negatives

It is also called an **Error Matrix**.

---
## 2. Structure of Confusion Matrix

| Actual / Predicted | Predicted 0 | Predicted 1 |
|---|---|---|
| Actual 0 | TN | FP |
| Actual 1 | FN | TP |

Where:

- **TN (True Negative)** → Model predicted No, and actual value is No
- **TP (True Positive)** → Model predicted Yes, and actual value is Yes
- **FN (False Negative)** → Model predicted No, but actual value is Yes  
  (**Type II Error**)
- **FP (False Positive)** → Model predicted Yes, but actual value is No  
  (**Type I Error**)

---

## 3. Accuracy

Accuracy tells how many predictions are correct out of total predictions.

### Formula:
- Accuracy = (TP + TN) / (TP + TN + FP + FN)
---

## 4. Error Rate

Error rate tells how many predictions are wrong.

Formula:
- Error = (FP + FN) / (TP + TN + FP + FN)
---

## 5. Recall (Sensitivity)

Recall measures how many actual positive cases are correctly identified.
It is important when reducing False Negatives is critical.

Example:
Disease Detection
Spam Detection
Fraud Detection
Formula:
- Recall = TP / (TP + FN)

- Higher Recall → Lower False Negatives
---

## 6. Precision

Precision measures how many predicted positive cases are actually correct.
It is important when reducing False Positives matters.

Example:
Cancer Detection
Loan Approval
Email Spam Detection
Formula:
- Precision = TP / (TP + FP)

- Higher Precision → Lower False Positives
---

## 7. F1-Score

F1-Score is the harmonic mean of Precision and Recall.

- It is useful when:
- Dataset is imbalanced
- Both FP and FN are important
- Domain knowledge is limited
Formula:
- F1 Score = 2 * (Precision * Recall) / (Precision + Recall)
---

## 8. Python Implementation
Libraries Used
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

- from sklearn.model_selection import train_test_split
- from sklearn.linear_model import LogisticRegression
- from sklearn.metrics import confusion_matrix
- from sklearn.metrics import precision_score
- from sklearn.metrics import recall_score
- from sklearn.metrics import f1_score
---


10. Key Learning
Accuracy alone is not enough for classification problems
Confusion Matrix gives deeper understanding of model performance
Recall helps reduce False Negatives
Precision helps reduce False Positives
F1-Score balances both Precision and Recall
Choosing the right metric depends on the problem statement
---

## Conclusion

Confusion Matrix and evaluation metrics help us select better models for real-world classification problems.
Instead of focusing only on accuracy, we should understand:

When Recall is important
When Precision is important
When F1-Score should be used

This leads to better decision-making in Machine Learning projects.
