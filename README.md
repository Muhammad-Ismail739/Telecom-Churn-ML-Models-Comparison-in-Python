# Telecom-Churn-ML-Models-Comparison-in-Python
# Overview



This project is centered on using machine learning to predict customer attrition for a telecommunications company. Customer attrition is when customers stop using a company’s services, which is also referred to as churn. The goal of this project is to analyze the primary drivers of customer attrition/disconnection, and build predictive models that will assist the telecommunications company in retaining customers.

Throughout this project, a number of data pre-processing, visualization, and modeling evaluation methods are employed to generate valuable business insights and improve decision-making.

# Project Goals

The main goals for this project are to:
1. Understand the distribution and patterns of customer attrition/churn through Exploratory Data Analysis (EDA) and then moving towards ML models.
2. Identify primary drivers of customer disconnection/attrition.
3. Evaluate and compare multiple modeling approaches to predict customer attrition.
4. Provide actionable insights to the business to improve customer retention.



# Dataset 

The dataset contains several customer-related parameters: tenure, contract type, payment type, internet service type, and churn status. These are typical of telecom customer data and have one record per customer and one record for each of their relationships. 
Kaggle Dataset Link: https://www.kaggle.com/datasets/abdullah0a/telecom-customer-churn-insightsfor-analysis

# Data Preprocessing 
Preprocessing was done prior to modeling. Below is a summary of those preprocessing steps: 
Address missing values and duplicates. 
Encode categorical features as numbers. 
Normalize numerical features when needed. 
Split the full dataset into a training dataset and a testing dataset to prep for evaluation of the model. 

# Exploratory Data Analysis (EDA) 
EDA was performed so we could understand how the data was behaving, and if we could observe any patterns or relations. We created several visualizations, including: 
Customer Tenure distribution: Most customers were churned in the 1st year. 
Internet Service Churn rate: Churn was considered for different types of internet service. 
Payment Methods and Contract-Based Customers: We found that month-to-month customers had a great deal of churn, and we can consider different payment methods if warranted. 



# Machine Learning Models 
Trained several models, compared performance, and made predictions for churn: 

1. Logistic Regression. 
2. Random Forest Classifier. 
3. Gradient Boosting Classifier. 
4. Support Vector Machine (SVM).

| Model               | Accuracy | Precision | Recall | F1-Score | AUC  |
| ------------------- | -------- | --------- | ------ | -------- | ---- |
| Logistic Regression | 0.88     | 0.88      | 1.00   | 0.94     | 0.52 |
| Random Forest       | 0.85     | —         | —      | —        | —    |
| Gradient Boosting   | 0.84     | —         | —      | —        | —    |
| SVM                 | 0.87     | —         | —      | —        | —    |


# Key Takeaways
The logistic regression model produced the best metrics of 88% accuracy and 100% recall, indicating its effectiveness in capturing nearly all customers identified as at-risk for churn. The model did exhibit some propensity to overpredict churn, indicating a small number of false positive predictions.
Customers with shorter tenure and customers on month-to-month plans were found to be more likely to churn. 
Payment type and internet service also accounted for differences in churn behavior (in the form of confusion).

# Summary
The project provides a demonstration of the application of machine learning to understand customer behavior in order to mitigate churn for telecom service providers. The logistic regression model achieved the optimal combination of metrics to represent the data while providing the accuracy to interpret some of the customer behavior and predict retention. With proper machine learning implementation the model would be beneficial to aid retention strategies and improve revenue.


# Author
Muhammad Ismail Saleem
