# 💼 Employee Financial Health Prediction

A machine learning project that analyzes employee financial data, engineers meaningful financial indicators, and predicts whether an employee has **Good Financial Health** using **Logistic Regression**.

---

## 📌 Project Overview

Financial well-being plays a crucial role in employee productivity and overall quality of life. This project leverages employee financial data to:

* Perform Exploratory Data Analysis (EDA)
* Identify spending and saving patterns
* Engineer financial health indicators
* Build a classification model to predict employee financial health
* Evaluate model performance using standard ML metrics

---

## 🎯 Objective

The primary goal is to classify employees into:

* **1 → Financially Healthy**
* **0 → Financially Unhealthy**

based on their salary, savings, investments, expenses, and loan obligations.

---

## 📂 Dataset Features

The dataset contains employee financial information such as:

* Monthly Salary
* Profit
* Savings Amount
* Investments
* EMI / Loan Payments
* Total Expenditure
* Rent Expenses
* Entertainment Expenses
* Other Deductions
* Other Expenses

Personal identifiers such as Employee ID and Name are removed before modeling.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 📊 Exploratory Data Analysis

### Data Inspection

* Dataset overview
* Statistical summaries
* Missing value detection
* Duplicate record analysis

### Visualizations

* Histograms for numerical feature distributions
* Correlation heatmaps
* Boxplots for outlier detection
* Scatterplots to analyze feature relationships

### Key Analyses

* Salary vs Profit
* Salary vs Savings
* Expenditure vs Profit
* Financial variable correlations

---

## ⚙️ Feature Engineering

A custom **Financial Health Score** is created using:

```python
FinancialHealthScore = (
    Profit * 0.35
    + Savings * 0.25
    + Investments * 0.20
    - EMI * 0.10
    - Expenditure * 0.10
)
```

Employees with scores above the median are classified as financially healthy.

### Additional Engineered Features

* Savings Ratio
* Expense Ratio
* EMI Burden
* Investment Ratio

These features help capture spending, saving, and debt behavior more effectively.

---

## 🤖 Machine Learning Model

### Algorithm Used

**Logistic Regression**

Chosen because:

* Simple and interpretable
* Effective for binary classification
* Fast training and prediction

### Data Preprocessing

* One-Hot Encoding for categorical variables
* Feature Scaling using StandardScaler
* Train-Test Split (80:20)

---

## 📈 Model Evaluation

The model is evaluated using:

* Accuracy Score
* Classification Report
* Confusion Matrix

Metrics analyzed include:

* Precision
* Recall
* F1-Score
* Overall Accuracy

---

## 📁 Project Structure

```bash
├── employee.ipynb
├── Employee_data.csv
├── requirement.txt
└── README.md
```

---

## 🚀 Installation & Setup

### Clone Repository

```bash
git clone https://github.com/yourusername/employee-financial-health-prediction.git

cd employee-financial-health-prediction
```

### Install Dependencies

```bash
pip install -r requirement.txt
```

### Run Notebook

```bash
jupyter notebook
```

Open:

```bash
employee.ipynb
```

---

## 📌 Future Improvements

* Random Forest Classification
* XGBoost Implementation
* Gradient Boosting Models
* Support Vector Machines
* Hyperparameter Tuning
* Streamlit Dashboard Deployment
* Advanced Feature Engineering
* Financial Health Risk Scoring System

---

## 📷 Key Insights

* Higher savings ratios generally correlate with better financial health.
* Excessive EMI burden negatively impacts financial stability.
* Investments and profits contribute significantly to financial well-being.
* Total expenditure shows an inverse relationship with financial health.

---

## 👩‍💻 Author

**Romya Jain**

Data Analytics & Machine Learning Enthusiast

📧 [romya.cse28@gmail.com](mailto:romya.cse28@gmail.com)

---

⭐ If you found this project useful, consider giving the repository a star!
