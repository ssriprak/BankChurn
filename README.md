# 🏦 Bank Customer Churn Prediction

This project analyzes and predicts customer churn for a retail bank using real-world data. It includes both a comprehensive **exploratory data analysis (EDA)** and the application of **machine learning models** to identify which customers are most likely to leave the bank.

---

## 📂 Dataset Overview

**Source:** `Churn Modeling.csv`  
**Target:** `Exited` — 1 if the customer churned, 0 otherwise  
**Features Used:**

- Demographics: `Geography`, `Gender`, `Age`
- Engagement: `Tenure`, `NumOfProducts`, `IsActiveMember`
- Financial: `CreditScore`, `Balance`, `EstimatedSalary`
- Behavioral: `HasCrCard`

---

## 📊 Part 1: Exploratory Data Analysis (EDA)

A detailed analysis was conducted to understand patterns and trends in the churn behavior.

### 🔍 EDA Highlights:

- **Univariate Analysis:**  
  Distributions of age, balance, salary, gender, and geography  
- **Bivariate Analysis:**  
  Churn rates by gender, geography, credit card ownership, activity status, number of products  
- **Boxplots:**  
  Comparisons of balance, salary, and age across churned vs retained users  
- **KDE Plots:**  
  Smoothed distributions of key variables segmented by churn status  
- **Correlation Heatmap:**  
  To detect multicollinearity and strong feature relationships

### 📈 Key Insights:

- Customers in **Germany** have higher churn rates  
- **Older** and **inactive** customers churn more  
- A surprisingly large number of high-balance customers churn  
- `NumOfProducts` and `IsActiveMember` are strong churn indicators

---

## 🤖 Part 2: Predictive Modeling

Three models were trained using the cleaned and encoded dataset:

### ⚙️ Models Implemented:

1. **Logistic Regression**  
2. **Random Forest Classifier**  
3. **XGBoost Classifier**

### 🔧 Pipeline Includes:

- One-hot encoding for categorical variables  
- Feature scaling for numerical inputs  
- Train/test split (70/30 stratified)  
- ROC curve, confusion matrix, and classification report

### 📊 Metrics Evaluated:

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- ROC AUC Score  
- Confusion Matrix  
- ROC Curve Visualization

---

## 🧠 Business Value

By identifying high-risk customers with these models, the bank can:

- Launch retention campaigns for specific demographics  
- Monitor high-value customers with churn tendencies  
- Improve customer experience strategies using data insights

---

## 🛠️ Tools & Libraries

- **Python**, **Pandas**, **Matplotlib**, **Seaborn**  
- **Scikit-learn**, **XGBoost**  
- Optional: **Tableau** for dashboard visualizations

---

## 🚀 How to Run

1. Clone this repository  
2. Add the `Churn Modeling.csv` file to the root directory  
3. Run the EDA notebook: `bank_churn_eda.ipynb`  
4. Run the ML script or notebook: `bank_churn_modeling.py` or `bank_churn_modeling.ipynb`

---

_“Turning data into decisions. One churned customer at a time.”_
