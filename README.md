# 📉 Customer Churn Analysis & Prediction using Machine Learning

This project focuses on analyzing customer churn behavior in the telecom industry using a real-world dataset. We explore churn patterns with detailed visualizations, quantify business impact, and train a machine learning model to predict churn with strong performance.

---

## 📂 Dataset Overview

The dataset contains information about **7,043 customers**, including:
- 🧍 Demographic details (gender, senior citizen status, partner, dependents)
- 🛠️ Service subscriptions (Internet, phone, streaming)
- 💳 Billing information (contract type, charges, payment methods)
- 🎯 Churn status (whether the customer left the service)

## 📊 Exploratory Data Analysis (EDA)
We begin by analyzing churn patterns across multiple variables to uncover actionable insights.

### 🔸 Churn Distribution
[Churn Distribution](https://github.com/user-attachments/assets/626d43ff-df2f-44a1-9995-0bc8dc79d78d)


> **~26.6%** of customers churned.  
> The dataset shows moderate imbalance.

### 🔸 Churn by Contract Type

([Churn by Time](https://github.com/user-attachments/assets/ff96d776-0edd-4f26-ae02-9a425ec4d879)
)
> Month-to-month customers have the **highest churn rate**, while yearly contracts reduce churn significantly.

### 🔸 Churn Rate by Tenure

![Churn rate by customer tenure](images/Churn%20rate%20by%20customer%20tenure.png)
> Short-tenure customers are most likely to churn.  
> Retention improves as tenure increases.

---

## Revenue Impact of Churn

We estimated the **business revenue loss** due to churn.
![Revenue lost due to churning](images/Revenue%20lost%20due%20to%20churning.png)

- **Total Revenue Lost**: `$2,862,926.90`
- **Avg Revenue per Churned Customer**: `$1,531.80`
- **Monthly Revenue Impact**: `$139,130.85`

## 🧹 Data Preprocessing

- Converted `TotalCharges` to numeric (handling empty strings)
- Imputed missing values using the **median**
- Applied **Label Encoding** to categorical features
- Scaled numerical features using **StandardScaler**
- Removed `customerID` column (irrelevant for prediction)

## 🧠 Model Building

We trained a **Random Forest Classifier** using the preprocessed data.
### ⚙️ Steps:
- 80/20 train-test split
- Feature scaling
- Model training using:
  ```python

RandomForestClassifier(random_state=42)
              precision    recall  f1-score   support

No Churn        0.83        0.90      0.86      1033
Churn           0.64        0.48      0.55       374

Overall Accuracy: 0.79

## Confusion Matrix
🔹 Most non-churners are correctly classified
🔸 Some churners are still missed, highlighting room for improvement

## Key Learnings
Identified churn patterns with EDA and visual storytelling
Quantified financial impact of customer attrition
Applied data preprocessing & encoding techniques
Built and evaluated a machine learning model from scratch

### Let’s Connect
If you’re a recruiter, mentor, or ML enthusiast, feel free to connect and share feedback.
I’m passionate about building data-driven solutions for real-world problems.
Let’s fight churn — one prediction at a time!




