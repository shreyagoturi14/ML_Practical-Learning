# Imbalanced Dataset Handling (Random Under Sampling & Random Over Sampling)

This project explains how to handle an **Imbalanced Dataset** using **Random Under Sampling** and **Random Over Sampling** techniques with Python and the `imblearn` library.

It helps improve classification model performance when one class has significantly more samples than the other.
---

## 1. What is an Imbalanced Dataset?
An imbalanced dataset occurs when the target variable classes are not equally distributed.

### Example:
Purchased
0    257
1    143
Here:

Class 0 has 257 samples
Class 1 has 143 samples
This creates imbalance and may lead to biased model predictions.

## 2. Why is it a Problem?
When the dataset is imbalanced:

The model becomes biased toward the majority class
Accuracy may look high but predictions may be poor
Minority class predictions become weak
Important positive cases may be missed

This is common in:
Fraud Detection
Disease Prediction
Spam Detection
Loan Default Prediction

## 3. Logistic Regression on Original Imbalanced Data
Model Accuracy
Accuracy = 88.75%
Even though accuracy looks high, the model may still perform poorly for the minority class.

## 4. Random Under Sampling
Random Under Sampling reduces the majority class samples to match the minority class.
Before Sampling
0 → 257
1 → 143
After Under Sampling
0 → 143
1 → 143
This creates a balanced dataset by removing extra majority samples.

## 5. Python Implementation (Under Sampling)
from imblearn.under_sampling import RandomUnderSampler
ru = RandomUnderSampler()
ru_x, ru_y = ru.fit_resample(x, y)
Model Accuracy After Under Sampling
Accuracy = 81.03%
Although accuracy decreases slightly, model fairness improves.

## 6. Random Over Sampling
Random Over Sampling increases the minority class samples to match the majority class.
After Over Sampling
0 → 257
1 → 257
This creates balance by duplicating minority class samples.

## 7. Python Implementation (Over Sampling)
from imblearn.over_sampling import RandomOverSampler
ro = RandomOverSampler()
ro_x, ro_y = ro.fit_resample(x, y)
Model Accuracy After Over Sampling
Accuracy = 81.03%
This helps the model learn minority class patterns better.

## 8. Comparison
Method	Class Distribution	Accuracy
Original Data	257 : 143	88.75%
Under Sampling	143 : 143	81.03%
Over Sampling	257 : 257	81.03%

## 9. Key Learning
Accuracy alone should not be trusted in imbalanced datasets
Balancing classes improves model reliability
Under Sampling removes extra majority samples
Over Sampling duplicates minority samples
Better evaluation should include Precision, Recall, and F1-Score

## 10. Libraries Used
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from imblearn.under_sampling import RandomUnderSampler
from imblearn.over_sampling import RandomOverSampler

## Conclusion
Imbalanced datasets can make machine learning models biased and unreliable.

Using:
Random Under Sampling
Random Over Sampling

helps improve classification performance and creates better model balance.
Choosing the right sampling technique depends on the dataset and business problem.
