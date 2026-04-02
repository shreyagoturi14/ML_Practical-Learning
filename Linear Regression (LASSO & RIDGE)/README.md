# Regularization in Machine Learning (Lasso & Ridge)

This project demonstrates the concept of **Regularization** using **Lasso (L1)** and **Ridge (L2)** regression techniques to improve model performance and reduce overfitting.

---

## Project Overview

In this project, I applied regularization techniques on a housing dataset to:

- Improve model generalization  
- Reduce overfitting  
- Compare Linear Regression, Lasso, and Ridge models  
- Analyze feature importance using model coefficients  

---

## Concepts Covered

### 🔹 1. Linear Regression (Baseline Model)
- Used as a reference model  
- Trained on all features  
- Evaluated using accuracy and error metrics  

---

### 🔹 2. Ridge Regression (L2 Regularization)

- Adds penalty on squared coefficients  
- Reduces magnitude of coefficients (but not zero)  
- Helps handle multicollinearity  


---

### 🔹 3. Lasso Regression (L1 Regularization)

- Adds penalty on absolute values of coefficients  
- Can shrink some coefficients to **zero**  
- Performs **feature selection automatically**  


---

## Data Preprocessing

- Removed unnecessary column (`date`)  
- Checked missing values  
- Applied **StandardScaler** for feature scaling  
- Split data using `train_test_split`  

---

## Exploratory Data Analysis (EDA)

- Correlation heatmap to understand relationships  
- Identified highly correlated features  
- Helped justify need for regularization  

---

## 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## Project Workflow

1. Loaded housing dataset  
2. Dropped irrelevant columns  
3. Checked missing values  
4. Performed correlation analysis  
5. Applied feature scaling  
6. Split data into training and testing sets  
7. Trained models:
   - Linear Regression  
   - Lasso Regression  
   - Ridge Regression  
8. Evaluated models using:
   - Mean Squared Error (MSE)  
   - Mean Absolute Error (MAE)  
   - Root Mean Squared Error (RMSE)  
9. Compared coefficients across models  

---

## Model Comparison

| Model | Purpose |
|------|--------|
| Linear Regression | Baseline model |
| Lasso Regression | Feature selection (removes less important features) |
| Ridge Regression | Reduces coefficient magnitude |

---

## Key Observations

- Linear Regression may overfit with many features  
- Lasso reduces some coefficients to zero → feature selection  
- Ridge reduces coefficient values but keeps all features  
- Regularization improves model stability and performance  

---

## ⚠️ Notes

- Convergence warning observed in Lasso  
  ✔ Can be solved by:
  - Increasing iterations  
  - Scaling data properly  
  - Adjusting alpha value  

---

Rgularization-ML/
│
├── regularization_lasso_ridge.ipynb
├── dataset/
│ └── housing.csv
├── README.md

