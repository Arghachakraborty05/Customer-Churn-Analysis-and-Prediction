# Customer-Churn-Analysis-and-Prediction Using Logistic Regression

## Project Overview

Customer churn is a critical challenge for subscription-based businesses, directly impacting revenue and long-term sustainability.  
This project focuses on **analyzing customer behavior** and **predicting churn risk** using historical customer data.

The objective is to **identify high-risk customers early** and support **data-driven retention strategies** through interpretable analytics and predictive modeling.

---

## Project Objectives

- Analyze customer behavior to identify key churn drivers  
- Identify high-risk customer segments  
- Build an interpretable churn prediction model  
- Generate churn probability scores to support business decisions  

---

## Dataset Description

The dataset contains **7,000+ customer records** with information related to:

- **Demographics:** gender, senior citizen status, dependents  
- **Account information:** tenure, contract type  
- **Services subscribed:** internet, streaming, security, and support services  
- **Billing and payment details**  
- **Churn status** (target variable)

### Target Variable

- **Churn**
  - `1` → Customer churned  
  - `0` → Customer retained  

---

## Data Preparation

Key preprocessing steps include:

- Handling missing values  
- Converting numerical fields stored as text  
- Encoding categorical variables  
- Feature scaling for model stability  
- Creating analytical features such as **tenure groups** and **customer segments**  

These steps ensure data consistency and modeling reliability.

---

## Exploratory Data Analysis (EDA)

EDA was conducted to uncover churn patterns and generate business insights, including:

- Churn rate across tenure groups  
- Impact of contract type and payment method on churn  
- Revenue impact of churned customers  
- High-risk contract and payment combinations  
- Customer segmentation based on risk and value  

These insights explain **why customers churn**, not just **who churns**.

---

## Statistical Validation

A statistical hypothesis test (**t-test**) was used to compare monthly charges between churned and retained customers.  
The results confirmed a **statistically significant difference**, validating observed churn patterns.

---

## Tools & Technologies

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Google Colab

---

## Churn Prediction Model

### Model Used
- **Logistic Regression**

### Why Logistic Regression?

- Produces churn probabilities (risk scores)  
- Highly interpretable and transparent  
- Suitable for business decision-making  
- Easy to monitor and deploy  

### Key Modeling Steps

- Stratified train-test split  
- Feature scaling using `StandardScaler`  
- Handling class imbalance  
- Threshold optimization based on **F1-score**  

---

## Model Evaluation

The model was evaluated using multiple metrics:

- **ROC–AUC Score:** ~0.84  
- Precision, Recall, F1-score  
- Confusion Matrix  
- ROC Curve  
- Churn Probability Distribution  
- Feature Importance (model coefficients)  

The evaluation emphasizes **balanced performance and business usability**, not accuracy alone.

---

## Model Output

The model generates:

### 1️. Churn Probability (Churn Score)
- A continuous value between **0 and 1** indicating churn risk  

### 2️. Binary Risk Classification
- High-risk vs Low-risk customers based on an optimized threshold  

### 3️. Feature Impact Explanation
- Identifies factors that increase or reduce churn likelihood  

### 4️. Aggregate Business Insights
- Percentage of customers at high risk  
- Estimated revenue exposure  
- Churn trends over time  

---

## Business Use Case

In real-world applications, the model functions as a **churn risk scoring system**:

- Run periodically (weekly or monthly) on active customers  
- Flag high-risk customers for proactive retention  
- Support targeted marketing and customer support actions  
- Reduce revenue loss due to churn  

The model acts as a **decision-support tool**, not a replacement for human judgment.

---

## Future Development

Potential enhancements include:

- Benchmarking against tree-based models (Random Forest, Gradient Boosting)  
- Incorporating **Customer Lifetime Value (CLV)**  
- Cost-sensitive threshold optimization  
- Monitoring data drift and retraining strategies  
- Deployment as a batch scoring pipeline or API service  
- Advanced explainability using **SHAP values**  

---

## Conclusion

This project demonstrates an **end-to-end churn analysis and prediction workflow**, combining business insights with interpretable machine learning.

The resulting churn risk scores provide **actionable intelligence** to support proactive customer retention and informed strategic decisions.

---
  
