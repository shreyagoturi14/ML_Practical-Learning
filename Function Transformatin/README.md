# 🔄 Function Transformation in Machine Learning

This project demonstrates the concept of **Function Transformation**, a technique used to transform data into a more suitable format for Machine Learning models.

Function transformation helps in handling skewed data, improving normality, and enhancing model performance.

---

##  What is Function Transformation?

Function Transformation is the process of applying mathematical functions to features in order to:
- Reduce skewness
- Normalize distributions
- Improve model performance
- Make relationships more linear

---

## Why Function Transformation is Important?

- Many ML algorithms assume normally distributed data
- Reduces the effect of extreme values
- Improves convergence of models
- Helps in better feature representation

---

## 🛠️ Types of Transformations Used

### 🔹 1. Log Transformation
- Used for right-skewed data
- Reduces large values
- Formula:
  log(x)
  
---

### 🔹 2. Square Root Transformation
- Reduces moderate skewness
- Works well for positive values
  √x

---

### 🔹 3. Square Transformation
- Expands smaller values
- Used when data is left-skewed
  x²

---

### 🔹 4. Reciprocal Transformation
- Strong transformation for highly skewed data
  1/x

  
---

## 📂 Project Workflow

1. Loaded dataset
2. Selected numerical features
3. Visualized original data distribution
4. Applied different transformations:
   - Log
   - Square Root
   - Square
   - Reciprocal
5. Compared distributions before and after transformation

---

## 📊 Visualization

Used plots such as:
- Histogram
- Distribution plots (KDE)
to understand the effect of transformations.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📊 Key Observations

- Log transformation effectively reduces right skewness
- Square root transformation smoothens data distribution
- Reciprocal transformation strongly compresses large values
- Proper transformation improves data quality for ML models

---


