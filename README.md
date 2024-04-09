startup-Acquisition-Status-Prediction.
Business Objective:


Methodology:
This section deals with the methodology followed to accomplish and achieve the goals of the project. Code snippets are shown here for reference purposes, but the entire code is available in the updated-Startup-Acquisition-Status-Prediction file. The methodology we followed is divided into main four parts: Data Collection, Data Preprocessing, EDA, Feature Engineering Data Modelling, pipeline, and Deployment

1. Data Collection:
The data provided by CrunchBase. Each row contains a Company’s Financial Information and is labeled with the company’s status (Operating, IPO, Acquired, Closed). This dataset is quite huge and thus it has 196553 rows and 44 columns.

2. Data Preprocessing:
Each row represents one company and has its financial information such as founded_at, description, category_code, funding_total_usd, etc, and labeled with the company’s status (Operating, IPO, Acquired, Closed)
removed unwanted columns which are irrelevant to our problem.
Checked and Removed the columns which have more than 98% of missing values.
Found and removed outliers from the funding_total_usd, relationship using the IQR method.
Converted category_code from  unique categories to  categories
Converted country_code from  unique categories to  categories.
Created ‘isClosed’ dependent column from the status column
Created active_days column from founded_at and closed_at column
Removed duplicate columns from the dataset
Removed irrelevant columns
3. EDA
4. Feature Engineering
Multicollinearity

Imbalance Dataset

Scaling

5. Modelling
Logistic Regression

Random Forrest Classifier

XGBoost

SVM

6. Pipeline
