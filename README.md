# Customer Churn Prediction - SyriaTel

## Author
**Hanifa Chepchirchir**  
**Facilitator:** Nikita Njoroge  
**Cohort:** Moringa School - DSFT-12

---

## Overview
SyriaTel, a leading telecom provider, is facing a high customer churn rate—losing approximately **15% of its customers annually**. This not only decreases revenue but also increases customer acquisition costs. This project leverages customer usage and service data to build predictive models that identify customers at risk of churning and uncover the key drivers behind their decisions.

---

## Problem Statement
SyriaTel lacks a proactive system to identify high-risk customers before they leave. With increasing churn impacting both **revenue** and **customer lifetime value**, the company needs a data-driven solution to forecast churn and retain valuable customers.

> **Objective:**  
> Build a classification model to predict customer churn and uncover key behavioral features contributing to churn.

---

## Project Objectives
- Explore customer data to understand churn trends
- Preprocess and engineer features for modeling
- Train and evaluate multiple classification models
- Identify key churn indicators
- Recommend business strategies based on insights

---

## Key Questions
- Can we predict churn based on customer behavior?
- What are the most influential features in predicting churn?
- How can SyriaTel use these insights to reduce churn?

---

## Dataset Description
The dataset contains telecom usage and account information for SyriaTel customers. Key features include:

- `international_plan`
- `voice_mail_plan`
- `number_vmail_messages`
- `customer_service_calls`
- `total_day_minutes`, `total_eve_minutes`, `total_night_minutes`, `total_intl_minutes`
- `total_day_charge`, `total_eve_charge`, `total_night_charge`, `total_intl_charge`
- `churn` (target variable: 1 = churned, 0 = retained)

---

## Models Used
- Logistic Regression
- Decision Tree (Untuned & Tuned)
- Random Forest Classifier
- XGBoost Classifier

---

## Model Evaluation

### ROC Curve Comparison
ROC curves were used to evaluate the performance of all models.  
> **AUC (Area Under Curve)** values reflect the model's ability to distinguish churners from non-churners — higher is better.

---

## Feature Importance (XGBoost & Logistic Regression)
The following features were identified as top drivers of churn:

- **No voicemail plan** → Higher churn risk  
- **Frequent customer service calls** → Indicate dissatisfaction  
- **International plan** → Customers more likely to churn  
- **High total day minutes/charges** → Linked to churn  
- **Charges** are more predictive than counts or durations

---

## Recommendations

### Targeted Retention Campaigns
- Focus on high-risk customers flagged by the model
- Upsell voicemail plans to users without them
- Review and improve international plan offerings

### Service Quality Monitoring
- Flag high-volume support users for early intervention
- Enhance responsiveness to customer complaints

### Product Bundling
- Bundle voicemail and international features into personalized plans to improve retention

---

## Next Steps
- **Feature Engineering Enhancements**: Add tenure, call pattern trends, and customer demographics  
- **Hyperparameter Tuning**: Use Bayesian optimization for improved performance  
- **Threshold Optimization**: Adjust probability thresholds for better balance between precision and recall  
- **Deployment**: Develop an API or integrate into CRM systems for real-time predictions

---

## Conclusion
This project demonstrates how predictive modeling can empower SyriaTel to reduce churn by identifying at-risk customers and acting proactively. With continued refinement and deployment, these insights can significantly boost customer retention and long-term profitability.



