#Customer Churn Analysis for a Telecommunications Company

Project Overview


This project focuses on analyzing customer churn for a telecommunications company, aiming to uncover factors driving churn and building predictive models to identify customers at risk of leaving.

Objectives:
Exploratory Data Analysis (EDA): Detect patterns, correlations, and trends within the dataset.
Data Preprocessing: Address missing values, encode categorical variables, and handle outliers to prepare the data for modeling.
Predictive Modeling: Create churn prediction models using Logistic Regression, Random Forest, and XGBoost.
Model Evaluation: Evaluate the models' effectiveness using performance metrics such as accuracy, precision, recall, and F1-score.
Actionable Insights: Deliver recommendations to help improve customer retention strategies.
Dataset

The dataset, sourced from a publicly available repository, provides details about customer demographics, account information, services utilized, and churn status.

Key Features:
customerID: Unique identifier for each customer.
gender: Gender of the customer.
SeniorCitizen: Indicates if the customer is a senior citizen (1 for Yes, 0 for No).
Partner: Specifies if the customer has a partner (Yes/No).
Dependents: Indicates whether the customer has dependents (Yes/No).
tenure: Number of months the customer has been with the company.
PhoneService: Whether the customer subscribes to phone service (Yes/No).
MultipleLines: Indicates if the customer has multiple phone lines (Yes/No/No phone service).
InternetService: Type of internet connection (DSL/Fiber optic/No service).
OnlineSecurity: Whether online security services are active (Yes/No/No internet service).
Churn: The target variable indicating if the customer left the company (Yes/No).
Analysis Process

1. Data Cleaning and Preprocessing
Missing values in the TotalCharges column, corresponding to customers with a tenure of 0 months, were replaced with 0.
Binary categorical variables (e.g., gender, Partner) were label-encoded.
Multi-class categorical variables (e.g., PaymentMethod) were converted using one-hot encoding.
2. Exploratory Data Analysis (EDA)
Created visualizations to analyze trends and patterns:
Churn Rate Analysis: Examined churn rates across categories such as gender and payment methods.
Correlation Heatmap: Highlighted relationships between numerical features and churn.
Identified key factors influencing churn, such as contract type and tenure.
3. Modeling and Evaluation
Developed and tested predictive models, including:

Logistic Regression
Random Forest Classifier
XGBoost Classifier
Naive Bayes
Assessed models using metrics like:

Accuracy
Precision
Recall
F1-Score
4. Insights and Recommendations
Customers with longer tenures and contracts like two-year plans are less likely to churn.
Senior citizens and customers without dependents have higher churn rates, indicating the need for targeted retention efforts.
Results

Model Performance (Post-Hyperparameter Tuning)
Random Forest Classifier

Accuracy: 75%
Precision (Non-churn): 88%
Recall (Non-churn): 77%
F1-Score (Non-churn): 82%
Precision (Churn): 52%
Recall (Churn): 72%
F1-Score (Churn): 61%
ROC AUC: 83%
XGBoost Classifier

Accuracy: 71%
Precision (Non-churn): 91%
Recall (Non-churn): 67%
F1-Score (Non-churn): 77%
Precision (Churn): 47%
Recall (Churn): 81%
F1-Score (Churn): 59%
ROC AUC: 82%
The ROC AUC scores indicate strong model performance in distinguishing between churned and non-churned customers.

Limitations

The dataset does not account for external factors such as market trends or economic conditions.
Additional feature engineering could further enhance model performance.
Future Work

Integrate external data to provide a more comprehensive analysis.
Develop advanced feature engineering techniques to capture complex relationships.
Explore cutting-edge machine learning models, such as neural networks, for better churn prediction.
