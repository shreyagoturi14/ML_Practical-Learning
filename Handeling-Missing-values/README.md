#  Handling Missing Values in Machine Learning

This project focuses on understanding and handling **missing data**, which is a crucial step in data preprocessing for Machine Learning.

Missing values can negatively impact model performance, so it is important to handle them properly before training models.

---

## 📌 What are Missing Values?

Missing values occur when no data is stored for a feature in a dataset.

Common reasons:
- Data not collected properly
- Human errors
- System failures
- Incomplete data entry

---

## 🚀 Techniques Used to Handle Missing Values

### 🔹 1. Removing Missing Values
- Dropping rows or columns with missing data
- Useful when missing values are very few

---

### 🔹 2. Mean / Median / Mode Imputation
- Replace missing values with:
  - Mean (for numerical data)
  - Median (for skewed data)
  - Mode (for categorical data)

---

### 🔹 3. Forward Fill / Backward Fill
- Fill missing values using previous or next values
- Useful in time-series data

---

### 🔹 4. Using Scikit-learn Imputer
- `SimpleImputer` used for automated handling
- Efficient and commonly used in ML pipelines

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn

---

## 📂 Project Workflow

1. Loaded dataset
2. Identified missing values
3. Visualized missing data
4. Applied different techniques:
   - Dropping missing values
   - Mean/Median/Mode imputation
   - Using SimpleImputer
5. Compared results before and after preprocessing

---

## 📊 Key Learnings

- Missing data must be handled before model training
- Different techniques are used based on data type
- Median is better for skewed data
- Removing data is not always the best option
- Proper preprocessing improves model accuracy

---

## ▶️ How to Run the Project

1. Clone the repository:

