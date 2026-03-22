# Feature Scaling in Machine Learning

This project focuses on understanding and implementing **Feature Scaling**, an essential preprocessing step in Machine Learning.

Feature scaling helps normalize the range of independent variables, improving the performance and convergence of ML models.

---

## 📌 What is Feature Scaling?

Feature Scaling is a technique used to standardize the range of features in a dataset so that no feature dominates others due to its scale.

It is especially important for algorithms like:
- K-Nearest Neighbors (KNN)
- Support Vector Machines (SVM)
- Gradient Descent-based models

---

## Types of Feature Scaling

### 🔹 1. Standardization (Z-score Normalization)
- Transforms data to have mean = 0 and standard deviation = 1
- Formula:
  
  z = (x - mean) / standard deviation

---

### 🔹 2. Normalization (Min-Max Scaling)
- Scales data to a fixed range [0,1]
- Formula:

  x' = (x - min) / (max - min)

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn

---

## 📂 Project Description

In this project:

- Loaded dataset using sklearn
- Identified numerical features
- Applied:
  - StandardScaler
  - MinMaxScaler
- Compared original vs scaled data
- Visualized the impact of scaling

---

## 📊 Key Observations

- Features with large ranges dominate smaller ones
- Scaling improves model performance
- Standardization works well for normally distributed data
- Normalization is useful when data has no clear distribution

---

## ▶️ How to Run

1. Clone the repository:

