📊 Customer Churn Prediction – AlphaCom Telecom
🏢 Business Context

AlphaCom, a major telecom provider, has recently experienced a concerning increase in customer churn. Despite offering competitive services, the churn rate continues to rise, affecting profitability and customer lifetime value. Traditional retention strategies are insufficient due to the complex interplay of factors like service usage, billing methods, contract types, and customer demographics. Without data-driven insights, AlphaCom continues to react to churn rather than prevent it.

🎯 Objective

As a Data Scientist at AlphaCom, the goal of this project is to:

Build a predictive machine learning model to identify high-risk churn customers

Analyze and interpret key drivers of churn

Enable proactive retention strategies

Reduce churn-related revenue losses

Enhance customer satisfaction and lifetime value

Strengthen AlphaCom’s competitive edge

📂 Dataset Description

The dataset contains demographic details, service usage patterns, account information, and customer status. The key attributes include:

Demographic Features

Gender, SeniorCitizen, Partner, Dependents

Account & Service Features

Tenure

PhoneService, MultipleLines

InternetService

OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport

StreamingTV, StreamingMovies

Contract, PaperlessBilling, PaymentMethod

Financial Features

MonthlyCharges

TotalCharges

Target Variable

Churn (Yes/No)

🔄 Project Workflow

The project follows a structured data science lifecycle:

Data Understanding
Loaded and reviewed the dataset to understand structure, variable types, and distributions.

Data Cleaning

Handled missing values (especially TotalCharges)

Corrected data types

Removed duplicates and inconsistencies

Exploratory Data Analysis (EDA)

Distribution plots for numeric and categorical features

Correlation analysis

Churn rate comparison across key attributes

Identification of top churn indicators

Feature Engineering

Encoding categorical variables

Scaling numerical features

Creating tenure groups, charge categories, etc.

Model Development
Tested multiple models:

Logistic Regression

Random Forest

XGBoost

Gradient Boosting

Model Evaluation
Used train-test split and evaluated models using:

Accuracy

Precision

Recall (priority metric for churn)

F1-score

ROC-AUC score

Model Deployment (Optional)
Prepared model pipeline for deployment (Pickle/Joblib).

📈 Key EDA Findings

Customers with month-to-month contracts show the highest churn.

Fiber optic users tend to churn more than DSL users.

Customers without tech support or online security have significantly higher churn.

Higher monthly charges are associated with increased churn.

Longer tenure strongly correlates with reduced churn.

🤖 Modeling Summary

XGBoost and Random Forest performed best.

The final chosen model achieved:

High recall → captures most churners

Strong accuracy and ROC-AUC

Feature importance revealed:

Contract type

Monthly charges

Tenure

Internet service type

Tech support availability

🔍 Business Insights

Short-term contract customers feel less committed and more likely to switch.

Lack of support services (TechSupport, OnlineSecurity) increases dissatisfaction.

High charges and poor perceived value contribute heavily to churn.

Early-tenure customers are at the highest risk—indicating onboarding issues.

🛠️ Recommendations

Based on analysis and modeling:

1. Retention Strategy

Introduce loyalty discounts for month-to-month users.

Provide incentives to switch to long-term contracts.

2. Service Improvement

Offer bundled support services (TechSupport + OnlineSecurity).

Improve quality and reliability of fiber optic service.

3. Pricing Optimization

Develop dynamic pricing or personalized offers for high-charge customers.

4. Customer Engagement

Proactively reach out to new customers within the first 3 months.

Create personalized recommendations based on service usage.

5. Operational Enhancements

Improve digital onboarding for paperless billing users.

Monitor payment methods; customers using electronic checks often churn more.

📦 Technologies Used

Python (Pandas, NumPy)

Matplotlib, Seaborn

Scikit-learn

XGBoost

Jupyter Notebook
