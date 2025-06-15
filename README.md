
# 🏦 Bank Customer Churn Prediction

This project analyzes data from ABC Multistate Bank to predict customer churn using machine learning. It includes exploratory data analysis (EDA), feature preprocessing, model building (Logistic Regression, Random Forest, XGBoost), and visualization of results including ROC curves and key metrics.

---

## 📂 Dataset

**Source**: Provided by ABC Bank  
**Target**: `churn` — whether the customer left (1) or stayed (0)  
**Features**:
- Demographic: age, gender, country
- Financial: credit score, balance, estimated salary
- Engagement: active member, tenure, products used, credit card

---

## 🔍 EDA Insights

- Churn rate visualized by age, country, gender, balance, and active membership
- Churned customers tend to have higher age and lower tenure
- High balance customers are more likely to churn (surprising insight)

---

## ⚙️ Modeling

Three models were trained and compared:
- **Logistic Regression**
- **Random Forest Classifier**
- **XGBoost Classifier**

Each model used a pipeline with:
- OneHotEncoding for categorical data
- StandardScaler for numerical features
- Model evaluation using accuracy, precision, recall, F1, and AUC

---

## 📈 Results

| Model               | Accuracy | Recall | ROC AUC |
|--------------------|----------|--------|---------|
| Logistic Regression| XX%      | XX%    | XX%     |
| Random Forest       | XX%      | XX%    | XX%     |
| XGBoost             | XX%      | XX%    | XX%     |

✅ ROC curves were plotted for comparison.  
✅ Feature importances from Random Forest and XGBoost help explain drivers of churn.

---

## 🛠️ Tech Stack

- Python (Pandas, Seaborn, Matplotlib, Scikit-learn, XGBoost)
- Jupyter Notebook
- Tableau (Optional)
- CSV dataset input

---

## 📌 How to Run

1. Clone the repo  
2. Add `bank_churn_data.csv` to the project folder  
3. Run the notebook or Python script  
4. (Optional) Export summary data to Tableau for dashboarding

---
