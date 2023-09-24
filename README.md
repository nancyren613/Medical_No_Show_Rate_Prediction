## Medical_No_Show_Rate_Prediction
 Develop machine learning model that predict patient’s probability of no-show and outline approach; based on  findings to give suitable recommendations would make to the operation unit efficiency
# Dataset
The data for this project mainly is patient medical appointment data with appointment history and no show status.
# Initial Setup
•	Libraries and modules related to data manipulation, visualization, and machine learning imported.
•	Data loaded from 'Medical_No_Shows.csv'.
# Exploratory Data Analysis(EDA)
•	Conducted a basic data overview to understand data shape and structure.
•	Data Quality Control:
  •	Checked data types and overall info.
  •	Examined uniqueness of columns.
  •	Evaluated missing value percentages.
  •	Checked for duplicates.
•	Feature Engineering:
  •	Created a binary 'NoShow' target column.
  •	Derived a 'LeadTime' feature (time between scheduling and appointment date).
  •	Engineered 'total_noshows_before' and 'total_appointments_before' features.
•	Data Insights:
  •	Highlighted data imbalance.
  •	Explored relationships:
      •	Age vs. NoShow
      •	LeadTime vs. NoShow
•	Statistical Tests:
  •	Assessed statistical significance of features against NoShow status.
•	Collinearity Check:
  •	Verified that numerical features are not strongly correlated.
# Modeling  
•	Feature Preparation:
  •	Defined numerical and categorical features.
  •	Converted categorical columns to string type.
  •	Split data into training and test sets (stratified based on target).
•	Benchmark Model - Logistic Regression
•	Tree-based Models:
  •	Random Forest
  •	XGBoost:
    •	Further examined training data.
    •	Checked value counts for categorical features.
# Summary
•	Three models (Logistic Regression, Random Forest, XGBoost) showed high performance:
  •	ROC-AUC score > 0.95.
  •	Precision and recall scores > 0.8.
•	Tree-based models outperformed Logistic Regression.
•	'total_noshows_before' and 'total_appointments_before' were top predictors.
•	Insights related to 'LeadTime' and 'Age' were highlighted.
•	Suggested model deployment as a web app using Flask on GCP.
•	Emphasized constant maintenance and monitoring of model performance.


