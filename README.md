# BetaGroup_JC_DS_FT_BDG_05_FinalProject

# **Telco Customer Churn Analysis and Machine Learning Model**

**By Beta Group** 
1. Khairunnisa Nur Afifah (JCDS0508-007)
2. Mayang Sari (JCDS0508-009)
3. Stefanus William Alexander (JCDS0508-017)

---

Tableau Dashboard: [View Dashboard](https://public.tableau.com/views/TelcoCustomerChurnDashboard_17413544666470/Home?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

Streamlit Deploy: [View Streamlit](https://telco-customer-churn-prediction-jcds0508.streamlit.app/) (Dummy for Streamlit : Telco Customer Churn - Dummy.csv)

## **Overview**

This project focus on analyzing customer churn in a telecommunication company (X) and developing a machine learning model to predict customer churn. By leveraging exploratory data analysis and predictive modeling, the goal is to uncover behavioral/service patterns influencing churn to refine retention strategies, develop a churn prediction model to proactively identify and retain high-risk customers, and provide actionable recommendations to reduce churn, boost retention, and also optimize promotional spending.

The analysis will be conducted using the Telco Customer Churn dataset. This dataset, uploaded by BlastChar on Kaggle, contains comprehensive records of telecommunications customers, with each row representing a customer attribute information and their churn status (churned or retained). The dataset is accessible [[here.](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)]

## **Objectives**

As a consultant, NexaData Solutions leverages advanced data analytics to:
- Identify churn drivers (e.g., service gaps, pricing pain points).
- Predict high-risk customers using machine learning.
- Deliver actionable retention strategies (e.g., targeted offers, service improvements).

This approach aims to reduce churn, enhance customer loyalty, and protect profitability for Telco Company X.

## **Dataset**

The dataset includes customer information such as:
- **Customer Demographics**: gender, SeniorCitizen, Partner, Dependents
- **Account Information**: customerID, tenure, Contract, PaperlessBilling
- **Financial Information**: PaymentMethod, MonthlyCharges, TotalCharges
- **Services Information**: PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies
- **Target Variable**: whether the customer churned (Yes or No)

## **Data Analysis and Insights**

**1. Exploratory Data Analysis (EDA)**
- Handling Incorrect Data Types: Idetified and processed inconsistent values
- Data Distribution: Visualized key variables using box plots
- Correlation Analysis: Measured relationshoips between numerical columns and churn

**2. Key Findings**
- Customers with month-to-month contracts are more likely to churn.
- Long-term customers (high tenure) are less likely to churn.
- Higher monthly charges correlate with higher churn.
- Fiber optic users have a higher churn rate, possibly due to higher service costs.

## **Machine Learning Model**

**1. Model Selection and Training**

Several models were tested, including:
- Logistic Regression
- Support Vector Machine (SVM)
- Catboost

**2. Model Evaluation**
- **Performance Metrics**: F2-score
- **Feature Importance**: Identified key predictors of churn

**3. Best Model and Results**

The Catboost model were tested twice, one with preprocessing and one with no preprocessing. The one without preprocessing performed best with:
- F2-score: ~75%
- Feature Importance: contract, tenure, and internet service were the top predictors

## **Business Recommendations**

- Encourage customers to switch to long-term contracts to reduce churn probability and maximize revenue.
- Offer loyalty programs or discounts to retain customers by implementing a tier rewards.
- Improve customer experience for fiber optic users by conducting a review of the pricing or improve service quality.
- Offer bundled packages that combine internet add-on services with both high and low churn rates.
