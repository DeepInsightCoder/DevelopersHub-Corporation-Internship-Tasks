#  Bank Loyalty Analyzer — Predicting Customer Churn

This project is part of my **Data Science & Analytics Internship** at **DevelopersHub Corporation**.  
The goal is to build a smart churn prediction system for a bank, identifying customers who are likely to leave based on their behavior and profile.



##  Objective

To develop a classification model that predicts whether a customer is likely to churn (leave the bank), so the bank can retain high-risk customers proactively.


##  Dataset

- **File:** `Churn_Modelling.csv`
- **Target Variable:** `Exited` (1 = churned, 0 = loyal)



##  Features Used

| Feature              | Description                          |
|----------------------|--------------------------------------|
| Age                  | Customer's age                       |
| EstimatedSalary      | Monthly income                       |
| CreditScore          | Credit score                         |
| Balance              | Account balance                      |
| NumOfProducts        | Number of bank products used         |
| Tenure               | Years with the bank                  |
| IsActiveMember       | Whether the user is active           |
| Geography_Germany    | One-hot encoded region               |
| Gender               | Encoded binary                      |
| HasCrCard            | Whether the user has a credit card   |
| Geography_Spain      | One-hot encoded region               |



##  Exploratory Data Analysis (EDA)

-  Countplot of churned vs loyal users
-  Age distribution by churn status
-  Heatmap showing feature correlations
-  Violin plots for salary and credit score trends



##  Preprocessing

- Removed non-predictive fields: `RowNumber`, `CustomerId`, `Surname`
- Encoded categorical features using:
  - `LabelEncoder` (for Gender)
  - `OneHotEncoding` (for Geography)
- Handled any missing data (none found)



##  Model Training

- **Algorithm:** Random Forest Classifier  
- **Split:** 80% training / 20% testing  
- **Accuracy Achieved:** **87%**



##  Evaluation

| Metric        | Value    |
|---------------|----------|
| Accuracy      | 87%      |
| Precision     | High for both churned and loyal |
| Recall        | Excellent for loyalty detection |



##  Feature Importance

Top features influencing churn:
1. `Age`
2. `EstimatedSalary`
3. `CreditScore`
4. `Balance`
5. `NumOfProducts`
6. `Tenure`
7. `IsActiveMember`
8. `Geography_Germany`

These insights can help banks focus their retention strategies better.
