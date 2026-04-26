# Naive Bayes Algorithm (Gaussian, Multinomial, Bernoulli)

This project demonstrates the implementation of the **Naive Bayes Algorithm** using different variants:
- Gaussian Naive Bayes  
- Multinomial Naive Bayes  
- Bernoulli Naive Bayes  

It focuses on classification problems and compares the performance of different Naive Bayes models.
---

## 1. What is Naive Bayes?
Naive Bayes is a **probability-based classification algorithm** based on **Bayes’ Theorem**.
It assumes that features are **independent** of each other (which is a “naive” assumption).

---
## 2. Bayes Theorem

P(A|B) = (P(B|A) * P(A)) / P(B)
Where:
P(A|B) → Posterior Probability
P(B|A) → Likelihood
P(A) → Prior Probability
P(B) → Evidence

## 3. Dataset Used
Features: cgpa, iq
Target: placement

## 4. Data Visualization
Scatter plot used to understand class distribution
Decision boundary visualization using mlxtend.plotting

## 5. Train-Test Split
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test = train_test_split(x, y, test_size=0.2, random_state=42)

## 6. Key Observations
GaussianNB performs best for continuous data
MultinomialNB is not ideal for this dataset
BernoulliNB performs poorly due to non-binary features
Choosing the correct variant is important
Visualization helps understand model behavior

## 7. Libraries Used
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.model_selection import train_test_split
from sklearn.naive_bayes import GaussianNB, MultinomialNB, BernoulliNB
from mlxtend.plotting import plot_decision_regions

## Conclusion

Naive Bayes is a simple yet powerful classification algorithm.
Works well on small datasets
Fast and efficient
Requires proper selection of variant based on data type
Understanding data type is key to getting good performance from Naive Bayes.


