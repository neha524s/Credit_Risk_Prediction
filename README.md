# Credit_Risk_Prediction

📌 Project Overview
- This project focuses on building a Credit Risk Prediction model using Lending Club loan data from 2014 to 2018. 
- The goal is to identify whether a borrower is likely to default or not, helping financial institutions reduce risk and improve decision-making.

📂 Dataset
- Source: Lending Club Loan Data (2014–2018)
- Target Variable: loan_status (binary — defaulted or not)

🔧 Preprocessing Steps
- Data Cleaning
- Dropped columns with more than 50% missing values.
- Handled remaining missing values using appropriate imputations.

📅 Feature Transformation
- Converted datetime features (like issue_d, last_pymnt_d) into meaningful numeric representations (e.g., number of months since issue).
- Applied encoding to categorical features, including:
- Weight of Evidence (WoE) transformation for monotonic relationship with the target.
- Information Value (IV) calculated to measure feature importance.
  
❌ Multicollinearity Handling
- Removed highly correlated features (VIF > threshold) to avoid multicollinearity issues.

⭐ Feature Importance
- Applied SelectFromModel using a Random Forest classifier to select top features based on importance scores.

🧠 Model Training
Logistic regression:
- Accuracy: 0.9739
- Recall: 0.9952
- F2 Score: 0.9910
- AUC: 0.9812

Random Forest:
- Accuracy: 0.9956
- Recall: 0.9991
- F2 Score: 0.9984
- AUC: 0.9985

Gradient Boosting:
- Accuracy: 0.9868
- Recall: 0.9992
- F2 Score: 0.9964
- AUC: 0.9955

Neural Network:
- Accuracy : 0.99565
