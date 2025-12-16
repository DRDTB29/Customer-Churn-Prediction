Customer Churn Prediction and Prevention is a telecom churn analytics notebook that cleans customer data, explores churn patterns, and trains machine learning models to predict which customers are likely to leave so that the business can take preventive actions.

Project objective
1. Uses a telecom customer dataset (7,000+ rows, 21 features) with demographics, services, charges, and a binary churn flag to understand why customers leave and to build a predictive model.
2. The goal is to support prevention strategies by identifying high‑risk customers based on patterns in tenure, billing, contract type, and services used.

Data preparation
1. Drops the customerID column, converts TotalCharges to numeric, fills missing values with the mean, removes tenure = 0 rows, and maps SeniorCitizen from 0/1 to No/Yes.
2. Encodes all categorical variables with LabelEncoder, scales features using StandardScaler, and splits into train and test sets for modeling.

Exploration and visualization
1. Examines distributions and outliers for tenure, MonthlyCharges, and TotalCharges, confirming no significant outliers after cleaning.
2. Visualizes churn vs gender, senior citizen, partner, dependents, internet and security services, contract type, payment method, and charges using pie charts, count plots, KDE plots, and boxplots to see which groups churn more.

Modeling and performance
1. Trains Logistic Regression, SVM, Decision Tree, Random Forest, and KNN classifiers on the processed data.
2. Compares them with cross‑validation; Logistic Regression achieves the best average score (about 0.80), with confusion matrices and classification reports used to evaluate churn vs non‑churn predictions.
 
