# 📘 Logistic Regression Algorithm (Machine Learning)

This project demonstrates the implementation of **Logistic Regression** for classification problems using Python and Scikit-learn.

It covers:
- Binary Classification (Single Input)
- Binary Classification (Multiple Input)
- Polynomial Logistic Regression
- Multiclass Classification using OVR and Multinomial methods

This project helps in understanding how Logistic Regression works for predicting categorical outcomes.

---

## 📌 Project Overview

In this project, I explored Logistic Regression for solving classification problems where the target variable is categorical (0/1 or multiple classes).

The workflow includes:
- Data loading and preprocessing
- Data visualization using scatterplots and pairplots
- Model training using Logistic Regression
- Decision boundary visualization
- Model accuracy evaluation
- Binary and multiclass classification

---

## Concepts Covered
---
###  1. Logistic Regression – Single Input

- One independent variable (Age)
- One dependent variable (Purchased)
- Binary classification problem (0 or 1)

Example:
Predicting whether a customer will purchase a product based on age.

📌 Learned:
- Sigmoid concept
- Classification prediction
- Accuracy score
- Decision boundary visualization

---

### 2. Logistic Regression – Multiple Input

- Multiple independent variables:
  - CGPA
  - IQ
- Target variable:
  - Placement (0 or 1)

Example:
Predicting student placement based on CGPA and IQ.

Learned:
- Multiple feature classification
- Model coefficients
- Intercept understanding
- Decision region plotting using `mlxtend`

---

### 3. Polynomial Logistic Regression

- Used when data is non-linear
- Applied using `PolynomialFeatures`

Example:
Placement prediction using:
- CGPA
- Placement Exam Marks

Learned:
- Non-linear decision boundary
- Polynomial feature transformation
- Better classification for complex patterns

---

### 4. Multiclass Logistic Regression

Used Iris dataset with 3 classes:

- Iris-setosa
- Iris-versicolor
- Iris-virginica

Methods used:

### OVR (One vs Rest)

- One class vs all remaining classes

### Multinomial Classification

- Direct multiclass classification

 Learned:
- Difference between OVR and Multinomial
- Pairplot visualization
- Species prediction

---

## Exploratory Data Analysis (EDA)

Performed:
- Scatterplots
- Pairplots
- Decision boundary visualization
- Class separation understanding

Used to understand whether data is linearly separable or requires polynomial transformation.
---
## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- mlxtend  
---
## 📂 Project Workflow

1. Loaded datasets
2. Removed unnecessary columns
3. Checked dataset structure using:
   - `.head()`
   - `.shape`
   - `.drop()`
4. Visualized data using plots
5. Defined features (X) and target (y)
6. Applied `train_test_split`
7. Trained model using `LogisticRegression`
8. Evaluated accuracy using `.score()`
9. Predicted outcomes using `.predict()`
10. Visualized decision boundaries

---

## Model Performance

### Single Input Logistic Regression
Accuracy: **91.25%**

### Multiple Input Logistic Regression
Accuracy: **85%**

### Polynomial Logistic Regression
Accuracy: **52.5%**

### Multiclass Classification
Accuracy: **100%**

---

## 📈 Key Observations

- Logistic Regression works well for binary classification
- Multiple inputs improve prediction understanding
- Polynomial features help with non-linear classification
- OVR and Multinomial both work well for multiclass problems
- Data visualization helps in selecting the right model
---
