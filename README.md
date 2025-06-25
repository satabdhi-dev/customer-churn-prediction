# 📉 Customer Churn Analysis with Machine Learning

This project analyzes customer churn patterns and builds a machine learning model to predict churn using a real-world telecom dataset. It combines Exploratory Data Analysis (EDA), Business Impact Estimation, and Predictive Modeling to uncover valuable insights for retention strategies.

---

## 🔍 Project Objectives

- Understand which customers are leaving (churning) and why.
- Visualize customer behaviors by contract type, tenure, and charges.
- Quantify revenue loss due to churn.
- Build and evaluate a churn prediction model.
- Identify the most influential features driving churn.

---

## 🧠 Dataset Overview

- 📦 **Rows**: 7043 customer records  
- 📊 **Target Variable**: `Churn` (Yes/No)  
- 🔑 **Features**: Contract type, tenure, payment method, monthly charges, etc.  

---

## 📊 Exploratory Data Analysis (EDA)

We begin by analyzing churn patterns across key variables.

### 🔹 Churn Distribution  
![Churn Distribution](churn-analysis-visualizations/Churn%20Distribution.png)  
> ~26.6% of customers have churned.  
> The dataset shows a moderate class imbalance.

---

### 🔹 Churn by Contract Type  
![Churn by Time](churn-analysis-visualizations/Churn%20by%20Time.png)  
> 📌 Customers with **month-to-month contracts** have the **highest churn rate**.  
> 🛡️ Yearly contracts significantly reduce churn.

---

### 🔹 Churn Rate by Tenure  
![Churn rate by customer tenure](churn-analysis-visualizations/Churn%20rate%20by%20customer%20tenure.png)  
> ⏳ Short-tenure customers are more likely to churn.  
> 📈 Retention improves significantly with longer tenure.

---

### 💸 Revenue Loss Due to Churn  
![Revenue lost due to churning](churn-analysis-visualizations/Revenue%20lost%20due%20to%20churning.png)  
> 💰 **Total Estimated Revenue Lost**: `$2,862,926.90`  
> 💸 **Avg. Revenue Lost per Churned Customer**: `$1,531.80`  
> 📆 **Approx. Monthly Loss**: `$139,130.85` if they had stayed

---

## 🤖 Model Building & Evaluation

We used a **Random Forest Classifier** for its robustness and ability to handle feature importance.

### 🔹 Confusion Matrix  
![Churn analysis confusion matrix](churn-analysis-visualizations/Churn%20analysis%20confusion%20matrix.png)  
> ✅ **Model Accuracy**: `79%`  
> ✅ Performs well for retained customers  
> ⚠️ Can be improved in identifying churned customers (Recall for Class 1: `0.48`)

---

### 🔹 Feature Importance  
![Churn Analysis Feature Importance](churn-analysis-visualizations/Churn%20Analysis%20Feature%20Importance.png)  
> 📌 **Top Predictors of Churn**:  
> - `TotalCharges`  
> - `MonthlyCharges`  
> - `Tenure`  
> - `Contract Type`

---

## 🔧 Future Improvements

- Try models like **XGBoost**, **Logistic Regression** for comparison  
- Apply **SMOTE** or **Class Weights** to handle class imbalance  
- Perform **Hyperparameter Tuning** with `GridSearchCV`  
- Deploy as an **interactive Streamlit Dashboard**

---

## 🧠 Key Learnings

- Real-world EDA with business-driven insights  
- Hands-on practice with missing data & encoding  
- Understanding churn behavior using visuals  
- Model building and evaluating with imbalanced classes  
- Communicating revenue impact through data


---

## 📬 Let's Connect!

💼 Looking for full-time Data Science or Machine Learning roles.  
🌐 [LinkedIn](https://www.linkedin.com/) | 📧 shizuku@email.com *(update this to your actual contact)*  
🎯 Passionate about using AI to solve real-world problems.

> ⭐ If you found this interesting, give the repo a star!






