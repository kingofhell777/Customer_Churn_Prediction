Customer churn is a major challenge for telecom companies because acquiring new customers is significantly more expensive than retaining existing ones. This project builds a machine learning model to predict whether a customer is likely to churn based on their service usage, contract details, and billing information.

The objective is to help businesses identify high-risk customers early and take preventive actions such as personalized offers, improved support, or retention campaigns.

**Dataset**

The project uses the Telco Customer Churn Dataset, which contains information about telecom customers and whether they discontinued their service.

Dataset characteristics:

Attribute	Description
Total Records	~7,000 customers
Total Features	21
Target Variable	Churn (Yes / No)
Important Features

tenure – Number of months the customer has stayed with the company

MonthlyCharges – Monthly subscription cost

TotalCharges – Total amount charged to the customer

Contract – Type of contract (Month-to-month, One year, Two year)

PaymentMethod – Customer payment method

InternetService – Type of internet service used

**Project Workflow
1. Data Preprocessing**

Removed non-informative identifiers (customerID)

Converted TotalCharges to numeric

Handled missing values

Encoded categorical variables

2.** Exploratory Data Analysis (EDA)**

Performed visual analysis to identify churn patterns.

Key visualizations:

Churn distribution

Contract type vs churn

Monthly charges vs churn

Feature correlation heatmap

3. **Feature Engineering
**
Transformed categorical variables into machine-readable format

Prepared dataset for machine learning models

4. **Model Training**

A Random Forest Classifier was trained on the dataset to predict customer churn.

**Steps:**

Train-test split (80/20)

Model training using Scikit-Learn

Performance evaluation

**5. Model Evaluation**

Model performance was evaluated using standard classification metrics.

Metric	Value
Accuracy	~79%
Model	Random Forest Classifier
Key Insights

Analysis of the dataset revealed several important churn indicators:

Customers with month-to-month contracts are more likely to churn

Customers with higher monthly charges tend to leave more frequently

Low tenure customers have the highest churn probability

Long-term contracts significantly reduce churn risk

These insights can help businesses improve customer retention strategies.

Technologies Used

Python

Pandas – Data manipulation

NumPy – Numerical computing

Matplotlib & Seaborn – Data visualization

Scikit-Learn – Machine learning
