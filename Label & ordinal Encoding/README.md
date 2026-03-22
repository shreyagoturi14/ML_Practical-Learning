# Label Encoding & Ordinal Encoding in Machine Learning

This project focuses on converting categorical data into numerical format using **Label Encoding** and **Ordinal Encoding**, which are essential preprocessing techniques in Machine Learning.

Since most ML algorithms cannot handle categorical data directly, encoding techniques are used to transform them into a suitable format.

---

## 📌 What is Categorical Data?

Categorical data represents features with discrete values such as:
- Colors (Red, Blue, Green)
- Sizes (Small, Medium, Large)
- Categories (Yes/No)

---

## Encoding Techniques Used

### 🔹 1. Label Encoding

- Converts categories into numerical labels
- Each unique category is assigned an integer value

#### Example:

| Category | Encoded |
|--------|--------|
| Red | 0 |
| Blue | 1 |
| Green | 2 |

📌 Suitable for:
- Binary categories
- When no ordinal relationship is required

---

### 🔹 2. Ordinal Encoding

- Assigns numerical values based on order or ranking

#### Example:

| Size | Encoded |
|------|--------|
| Small | 0 |
| Medium | 1 |
| Large | 2 |

📌 Suitable for:
- Ordered categories (ranking matters)

---

## ⚠️ Important Difference

| Feature | Label Encoding | Ordinal Encoding |
|--------|---------------|------------------|
| Order Considered | ❌ No | ✅ Yes |
| Use Case | Nominal Data | Ordered Data |

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn

---

## 📂 Project Workflow

1. Loaded dataset
2. Identified categorical columns
3. Applied:
   - Label Encoding using `LabelEncoder`
   - Ordinal Encoding using `OrdinalEncoder`
4. Transformed categorical data into numeric form
5. Compared original vs encoded data

---

## ⚙️ Implementation

### 🔹 Label Encoding

```python
from sklearn.preprocessing import LabelEncoder

le = LabelEncoder()
data['column'] = le.fit_transform(data['column'])
