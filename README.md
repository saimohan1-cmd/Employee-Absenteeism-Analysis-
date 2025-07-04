#  Employee Absenteeism Analysis

This project focuses on analyzing and predicting employee absenteeism using HR data. By examining various demographic and organizational attributes, we aim to understand what factors are most associated with absence and provide actionable insights for HR decision-making.

---

## Dataset

- **Source**: [Kaggle - HR Analytics Absenteeism Dataset](https://www.kaggle.com/datasets/HRAnalyticRepository/absenteeism-dataset)
- **File Used**: `MFGEmployees4.csv`
- **Key Columns**:
  - `Gender`
  - `Age`
  - `DepartmentName`
  - `Division`
  - `BusinessUnit`
  - `AbsentHours`

---

##  Objective

- Explore and visualize absenteeism patterns
- Build a predictive model to identify likely absentee employees
- Explain model predictions using SHAP for transparency

---

##  Steps Performed

### 1. **Data Cleaning**
- Removed irrelevant columns (e.g., names)
- Encoded categorical variables
- Handled missing data

### 2. **Feature Engineering**
- Created a binary column `Absenteeism`: `1` if `AbsentHours > 0`, else `0`

### 3. **Exploratory Data Analysis (EDA)**
- Visualized:
  - Absenteeism distribution
  - Age vs Absenteeism
  - Gender, Department, Division, and Business Unit vs Absenteeism

### 4. **Modeling**
- Trained a **Random Forest Classifier**
- Evaluated using accuracy, precision, recall, and F1-score

### 5. **Model Interpretability**
- Used **SHAP** to understand feature importance and individual predictions

---

## 📈 Key Insights

- Absenteeism is more influenced by **organizational** features (e.g., Division, Department) than by **personal** ones (like gender).
- A significant number of employees show **no absenteeism**, while others are absent at varying levels.
- The model identifies key departments and divisions prone to absenteeism.

---

## Tech Stack

- Python
  - Pandas, NumPy
  - Seaborn, Matplotlib
  - Scikit-learn
  - SHAP
- Jupyter Notebook

---


## Outcome

This project offers a data-driven way for HR teams to:
- Detect absenteeism patterns
- Predict future absenteeism
- Take proactive action to address high-risk groups

---

