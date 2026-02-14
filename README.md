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

* Source: SPARCS (Statewide Planning and Research Cooperative System) via Kaggle.Size: Original dataset contains 2.19 million rows; analysis performed on a representative sample.
* Key Features:Patient Demographics: Age Group, Gender, Race, Ethnicity.Clinical Data: CCSR Diagnosis/Procedure Codes, APR DRG Description, Severity of Illness, Risk of Mortality.
* Administrative Data: Facility Name, Type of Admission, Length of Stay, Payment Typology.
* Targets: Total Charges, Total Costs.

🛠️ Tech Stack

* Language: Python
* Libraries: Pandas, NumPy (Data Handling); Matplotlib, Seaborn (Visualization); Scikit-Learn (Machine Learning Pipeline).

🚀 Methodology

* Exploratory Data Analysis (EDA): Identified missing values ​​(eg, Birth Weight and Payment Typology 3 had >89% missing data) and removed duplicate entries.
* Preprocessing: Sampling of data for computational efficiency.Handling categorical variables via encoding.Standardization of numerical features.
* Modeling: Implemented a pipeline comparing Linear Regression and ensemble methods.
* Optimization: Tuned the Random Forest model to achieve peak performance.

📈 Key Results

* Top Performer: The Tuned Random Forest Regressor outperforms linear and boosting models.
* Accuracy: The final model explains over 90% of the variance (R^2 > 0.90) in hospital charges.

⚠️ Limitations

* The model relies on administrative data and does not include real-time clinical measurements.
* Dataset is specific to a certain region and time period; external systems may show different billing patterns.

👤 Author

Name: Nikhil Gopi
Organization: Entri Elevate
Date: February 14, 2026
