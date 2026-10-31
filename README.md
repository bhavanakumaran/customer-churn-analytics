# Customer Churn Analysis and Prediction

## Project Overview
This project analyzes customer churn in a telecommunications company using Python, exploratory data analysis, and machine learning.

The objective is to identify customer churn patterns, understand the factors associated with customer attrition, predict customers who are likely to churn, and suggest data-driven customer retention strategies.

## Objectives
- Analyze customer data to identify churn patterns.
- Explore the relationship between customer characteristics and churn.
- Build machine learning models to predict customer churn.
- Classify customers into Low, Medium, and High churn-risk categories.
- Derive business insights and recommend customer retention strategies.

## Technologies Used
- **Programming Language:** Python
- **Environment:** Jupyter Notebook
- **Data Analysis:** Pandas, NumPy
- **Data Visualization:** Matplotlib
- **Machine Learning:** Scikit-learn
- **Model Storage:** Pickle

## Dataset
The project uses the Telco Customer Churn dataset.

- Total records: 7,043 customers
- Original features: 21 columns
- Target variable: `Churn`
- Churned customers: 1,869
- Retained customers: 5,174
- Overall churn rate: 26.54%

## Project Workflow

### 1. Data Cleaning and Preprocessing
- Checked missing values and duplicate records.
- Converted data types where necessary.
- Prepared the dataset for analysis and modelling.

### 2. Exploratory Data Analysis
Analyzed churn patterns across:
- Contract types
- Tenure groups
- Payment methods
- Internet services
- Customer demographics
- Additional subscribed services
- Monthly and total charges

### 3. Data Visualization
Created visualizations to identify churn trends, customer distributions, revenue patterns, and model performance.

### 4. Feature Engineering and Model Preparation
- Encoded categorical variables using One-Hot Encoding.
- Applied feature scaling for Logistic Regression.
- Split the dataset into training and testing sets using an 80:20 ratio.

### 5. Machine Learning Models
Implemented and evaluated:
- Logistic Regression
- Random Forest Classifier

### 6. Model Evaluation

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 80.70% | 77.00% |
| Precision | 65.84% | 55.95% |
| Recall | 56.68% | 62.83% |
| F1-Score | 60.92% | 59.19% |

Logistic Regression was selected for the reusable prediction workflow based on its stronger accuracy, precision, and F1-score. Random Forest achieved higher recall.

### 7. Churn Prediction and Risk Classification
Developed a reusable prediction function that accepts customer information and returns:
- Churn prediction
- Churn probability
- Risk classification: Low, Medium, or High

### 8. Business Insights
Key findings include:
- Month-to-month contract customers had a churn rate of 42.7%.
- Customers in the New tenure group had a churn rate of 47.4%.
- Customers using electronic checks had a churn rate of 45.3%.
- Fiber optic customers had a churn rate of 41.9%.
- Customers without online security and technical support showed higher churn rates.

### 9. Customer Retention Recommendations
Based on the observed patterns, the project proposes:
- Improved onboarding for new customers.
- Incentives for longer-term contracts.
- Proactive technical support.
- Promotion of online security services.
- Review of pricing and service bundles.
- Encouragement of automatic payment methods.

## Business Impact
The historical charges associated with churned customers amounted to approximately **$2.86 million**.

Illustrative retention scenarios were also analyzed to estimate the historical charges represented by potentially retained customers. These figures are not forecasts of future revenue or profit.

## Project Structure

```text
customer-churn-analytics/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── notebooks/
│   └── churn_analysis.ipynb
│
├── models/
│   ├── logistic_regression_model.pkl
│   ├── standard_scaler.pkl
│   └── feature_columns.pkl
│
└── README.md
```

## Limitations and Future Improvements
- Experiment with additional machine learning algorithms.
- Improve churn recall and evaluate alternative classification thresholds.
- Perform further feature selection and model tuning.
- Test retention strategies using controlled experiments.
- Develop an interactive application for customer churn prediction.

## Conclusion
This project demonstrates an end-to-end customer churn analytics workflow, combining data cleaning, exploratory analysis, machine learning, risk classification, and business recommendations to support data-driven customer retention decisions.