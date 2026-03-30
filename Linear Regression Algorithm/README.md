# Linear Regression Algorithm (Machine Learning)

This project demonstrates the implementation of **Linear Regression** techniques using Python and Scikit-learn.  
It covers **Simple Linear Regression, Multiple Linear Regression, and Polynomial Regression** along with data visualization and model evaluation.

---

## Project Overview

In this project, I explored how different types of regression models work by applying them on real datasets and visualizing the results.

The workflow includes:
- Data loading and preprocessing
- Exploratory Data Analysis (EDA)
- Model training using Linear Regression
- Model evaluation and prediction
- Visualization of results

---

## Concepts Covered

### 1. Simple Linear Regression
- Relationship between one independent variable (CGPA) and dependent variable (Package)
- Visualized using scatter plot
- Fitted regression line

📌 Equation:
y = mx + c


---

### 2. Multiple Linear Regression
- Used multiple features:
  - YearsExperience
  - Age
- Predicted Salary
- Analyzed feature relationships using:
  - Pairplot
  - Correlation Heatmap

📌 Equation:
y = m1x1 + m2x2 + c


---

### 3. Polynomial Regression
- Used when data is non-linear
- Applied polynomial feature transformation (degree = 2)
- Captured curved relationships in data
Helps in modeling complex patterns

---

## Exploratory Data Analysis (EDA)

- Scatter plots for relationship visualization
- Pairplot for multi-feature analysis
- Heatmap for correlation analysis
- Distribution understanding of variables

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 📂 Project Workflow

1. Loaded datasets (Placement & Salary data)
2. Checked data using:
   - `.head()`
   - `.shape`
   - `.isnull().sum()`
3. Visualized relationships using plots
4. Defined features (X) and target (y)
5. Applied `train_test_split`
6. Trained model using `LinearRegression`
7. Evaluated model using `.score()`
8. Predicted values using `.predict()`
9. Visualized regression line and results

---

## Model Performance

- Simple Linear Regression Accuracy: ~77%  
- Multiple Linear Regression Accuracy: ~88%  
- Polynomial Regression used for non-linear data patterns  

---

## Key Observations

- Strong positive relationship between CGPA and Package  
- Salary increases with experience and age  
- Polynomial regression captures non-linear trends better  
- Feature relationships are highly correlated  

---

## 📁 Project Structure
Linear-Regression-ML/
│
├── linear_regression.ipynb
├── datasets/
│ ├── placement.csv
│ ├── salary_data.csv
│ └── salary_level.csv
├── README.md

## Learning Outcome

- Understood regression concepts clearly  
- Learned how to visualize data relationships  
- Gained hands-on experience with sklearn models  
- Built a strong foundation in supervised learning  

