# 📱 Customer Churn Prediction — Classification

A supervised machine learning project predicting customer churn using
Logistic Regression and Decision Tree classifiers.
Built as part of my Data Science learning journey.

---

## 📌 Project Overview

This project builds and compares two classification models trained on
7,043 Telco customer records to predict whether a customer will churn.
It covers the full ML workflow including cleaning, feature selection,
model training, evaluation, and comparison.

**Business Goal:** Identify customers likely to churn before they leave
so the business can intervene with targeted retention strategies.

---

## 📂 Dataset

- **Source:** [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/abbas829/telco-customer-churn-dataset)

---

## 🔑 Features Used

- tenure — how long the customer has been with the company
- MonthlyCharges — current monthly bill
- TotalCharges — total amount paid over tenure
- SeniorCitizen — whether the customer is a senior citizen

---

## 🛠️ What Was Done

- Loaded and inspected 7,043 customer records
- Converted TotalCharges from string to numeric
- Handled missing values created during conversion
- Selected numeric features using `select_dtypes`
- Split data 80/20 into training and test sets
- Trained Logistic Regression model
- Trained Decision Tree model with max_depth=5
- Evaluated both models using Accuracy, Precision, Recall, F1
- Visualised confusion matrices for both models
- Compared model performance and trade-offs

---

## 📊 Model Results

| Metric | Logistic Regression | Decision Tree |
|---|---|---|
| Accuracy | 0.78 | 0.77 |
| Precision | 0.62 | 0.58 |
| Recall | 0.44 | 0.47 |
| F1 Score | 0.51 | 0.52 |
| Churners caught | 163 | 175 |
| Churners missed | 211 | 199 |

Decision Tree caught more churners. Logistic Regression had fewer
false alarms. Neither is definitively better — it depends on the
business priority.

---

## 🧰 Tools & Libraries

- Python 3
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📁 File Structure
customer-churn-prediction/
│
├── analysis.ipynb        # Main ML notebook
├── telco_churn.csv       # Dataset
└── README.md             # Project documentation

---

## 💡 Key Learnings

- Accuracy alone is misleading on imbalanced datasets
- Recall matters more than precision for churn problems
- Decision Trees are more flexible but prone to false alarms
- Confusion matrix tells the full story accuracy hides
- Next step — try Random Forest or XGBoost to improve recall

---

## 👤 Author

**Lindokuhle Nyoka**
[GitHub](https://github.com/lk-nyoka) · [LinkedIn](https://linkedin.com/in/lindokuhle-nyoka-982019245)

