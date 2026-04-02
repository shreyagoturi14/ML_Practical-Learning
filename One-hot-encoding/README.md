## 🔢 One Hot Encoding in Machine Learning

This project demonstrates the concept and implementation of **One Hot Encoding**, a technique used to convert categorical data into numerical format for Machine Learning models.

Handling categorical variables properly is essential because most ML algorithms cannot work with non-numeric data.

---

## What is One Hot Encoding?

One Hot Encoding is a process of converting categorical variables into a binary (0 or 1) format.

Each category is transformed into a new column, and values are assigned as:
- **1** → if the category is present  
- **0** → if the category is not present  

---

## Why One Hot Encoding is Important?

- Machine Learning models require numerical input
- Prevents incorrect ordering of categories
- Avoids misleading relationships between categories
- Improves model performance

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn

---

## 📂 Project Workflow

1. Loaded dataset
2. Identified categorical features
3. Applied One Hot Encoding using:
   - `pandas.get_dummies()`
   - `OneHotEncoder` from sklearn
4. Compared original vs encoded data
5. Analyzed the transformed dataset

---

## ⚙️ Implementation Methods

### 🔹 Using Pandas

```python
pd.get_dummies(data)
