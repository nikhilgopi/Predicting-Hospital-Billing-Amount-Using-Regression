Predicting Hospital Billing Amount Using Regression Model

📌 Project Overview

In modern healthcare systems, hospital expenses vary significantly based on factors such as age, severity of illness, and duration of stay. This project utilizes machine learning to analyze historical hospital records and predict medical billing amounts. By providing data-driven cost estimations, this system aims to improve financial transparency for patients and optimize resource allocation for healthcare providers.

🎯 Objectives

* Analyze Relationships: Understand how patient characteristics and medical conditions influence billing costs.
* Data Preprocessing: Perform cleaning, feature engineering, and scaling to improve model accuracy.
* Model Benchmarking: Build and compare regression models, specifically Linear Regression and Random Forest Regressor .
* Performance Evaluation: Assess models using MAE, MSE, RMSE, and R^2 scores
* Feature Importance: Identify the most influential factors affecting hospital charges.

📊 Dataset Description

* Source: Hospital inpatient discharge dataset (https://www.kaggle.com/code/owentamunogilbert/new-york-hospital-charges-analysis/input)
* Records: ~650,000+ (sampled where required)
* Features: Patient demographics, clinical severity indicators, admission type, hospital details, and billing-related variables
* Target Variable:
* log_total_charges (log-transformed hospital billing amount)
Log transformation was applied to reduce skewness and improve model performance.

🛠️ Tech Stack

* Language: Python
* Libraries: Pandas, NumPy (Data Handling); Matplotlib, Seaborn (Visualization); Scikit-Learn (Machine Learning Pipeline).

🧹 Data Preprocessing

* Removed duplicate records.
* Handled missing values using appropriate strategies.
* Dropped leakage features (Total Charges, Total Costs).
* Applied log transformation to the target variable.
* Encoded categorical variables using One-Hot Encoding.
* Scaled numerical features using StandardScaler.
* Selected top 30 important features using Random Forest feature importance.

🔍 Exploratory Data Analysis (EDA)

Key insights:

* Hospital charges were highly right-skewed before log transformation.
* Length of Stay strongly correlates with hospital billing.
* Higher clinical severity leads to significantly higher costs.
* Emergency and trauma admissions show higher billing patterns.
* Demographic features have comparatively lower impact on costs.

🧠 Models Implemented

Five regression models were built and evaluated:

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor
* AdaBoost Regressor
* MLP Regressor

📈 Key Results

Model Performance Summary

| Model                     | R² Score |
|---------------------------|----------|
| Linear Regression         | 0.69     |
| Random Forest Regressor   | 0.89     |
| Gradient Boost Regressor  | 0.83     |
| AdaBoost Regressor        | 0.62     |
| MLP Regressor             | 0.84     |
| Tuned Random Forest       | 0.91     |


* Top Performer: The Tuned Random Forest Regressor outperforms linear and boosting models.
* Accuracy: The final model explains over 90% of the variance (R^2 > 0.90) in hospital charges after the Hyperparameter test.

⚠️ Limitations

* The model relies on administrative data and does not include real-time clinical measurements.
* Dataset is specific to a certain region and time period; external systems may show different billing patterns.

👤 Author

Name: Nikhil Gopi
Organization: Entri Elevate
Date: February 14, 2026
