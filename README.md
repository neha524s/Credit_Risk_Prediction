# Credit_Risk_Prediction

📌 Project Overview
This project focuses on building a Credit Risk Prediction model using Lending Club loan data from 2014 to 2018. The goal is to identify whether a borrower is likely to default or not, helping financial institutions reduce risk and improve decision-making.

📂 Dataset
Source: Lending Club Loan Data (2014–2018)

Includes loan records, borrower information, and loan status.

Target Variable: loan_status (binary — defaulted or not)

🔧 Preprocessing Steps
🧹 Data Cleaning
Dropped columns with more than 50% missing values.

Handled remaining missing values using appropriate imputations.

📅 Feature Transformation
Converted datetime features (like issue_d, last_pymnt_d) into meaningful numeric representations (e.g., number of months since issue).

Applied encoding to categorical features, including:

Weight of Evidence (WoE) transformation for monotonic relationship with the target.

Information Value (IV) calculated to measure feature importance.

🔍 Feature Engineering
✅ Target Correlation
Selected features based on their correlation with the target variable.

❌ Multicollinearity Handling
Removed highly correlated features (VIF > threshold) to avoid multicollinearity issues.

⭐ Feature Importance
Applied SelectFromModel using a Random Forest classifier to select top features based on importance scores.

🧠 Model Training
Algorithm used: Logistic Regression

Train/Test Split applied

Achieved an accuracy of 97% on the test data.
