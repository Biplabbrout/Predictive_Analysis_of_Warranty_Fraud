Warranty Claims Fraud Prediction
Project Overview
This project focuses on predicting whether warranty claims are genuine or fraudulent by analyzing various features such as region, product category, claim value, and more. The dataset, sourced from Kaggle, consists of 358 records with 21 attributes.

Data Dictionary

Column Name	Description
Unnamed: 0	Index
Region	Region where the claim originated
State	State where the claim was filed
Area	Area classification (Urban/Rural)
City	City where the claim was made
Consumer_profile	Type of consumer (Business or Personal)
Product_category	Product category (Household/Entertainment)
Product_type	Specific product (AC/TV)
AC_1001_Issue	Issue with AC component 1 (0 - No issue, 1 - Repair, 2 - Replacement)
AC_1002_Issue	Issue with AC component 2 (0 - No issue, 1 - Repair, 2 - Replacement)
AC_1003_Issue	Issue with AC component 3 (0 - No issue, 1 - Repair, 2 - Replacement)
TV_2001_Issue	Issue with TV component 1 (0 - No issue, 1 - Repair, 2 - Replacement)
TV_2002_Issue	Issue with TV component 2 (0 - No issue, 1 - Repair, 2 - Replacement)
TV_2003_Issue	Issue with TV component 3 (0 - No issue, 1 - Repair, 2 - Replacement)
Claim_Value	Value of the claim in INR
Service_Center	Code of the service center
Product_Age	Age of the product in days
Purchased_from	Source of purchase (Dealer, Manufacturer, Internet)
Call_details	Duration of customer care call
Purpose	Purpose of the call
Fraud	Fraudulent (1) or Genuine (0)
Key Insights
Through exploratory data analysis, several patterns emerged:

The southern region of India, notably Andhra Pradesh and Tamil Nadu, reported the highest number of warranty claims.

Urban areas like Hyderabad and Chennai recorded a greater number of fraudulent claims.

TVs had more warranty claims for personal use compared to ACs.

Some fraudulent AC claims were filed even when no parts had issues.

Fraudulent TV claims occurred both with and without part-related issues.

Purchases made directly from manufacturers were more likely to involve fraud.

Higher claim values were generally associated with fraudulent claims.

Service Center 13 had a disproportionately high number of fraudulent claims, despite fewer overall claims.

Calls shorter than 3–4 minutes were more frequently linked to fraudulent claims.

Modeling Approach
To predict fraudulent claims, three machine learning models were applied:

Decision Tree Classifier

Random Forest Classifier

Logistic Regression

All models achieved strong accuracy scores between 91–92%. However, due to the dataset’s limited size and the imbalance between fraudulent and genuine claims, the recall scores for fraud detection were relatively lower. This limitation highlights the need for a larger and more balanced dataset for improved model performance.

Conclusion
This project demonstrates the potential of machine learning in detecting fraudulent warranty claims. Implementing such predictive systems can lead to significant cost savings and greater efficiency in processing warranty claims.

