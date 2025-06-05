#  Health Cost Forecaster AI — Predicting Insurance Charges

This project is part of my **Data Science & Analytics Internship** at **DevelopersHub Corporation**.  
The objective is to predict medical insurance charges using customer demographic and health-related data using regression modeling.



##  Objective

To build a machine learning model that predicts the **expected medical charges** for a customer based on their:
- Age
- BMI
- Smoking habits
- Region
- Gender
- Number of children

This helps insurance companies forecast claim risk and create personalized premium plans.



##  Dataset

- **File Name**: `insurance.csv`
- **Rows**: 1338
- **Target Variable**: `charges` (Total medical expenses)

### Features:
| Column         | Description                             |
|----------------|-----------------------------------------|
| age            | Age of the person                       |
| sex            | Gender (Male/Female)                    |
| bmi            | Body Mass Index                         |
| children       | Number of children covered by insurance |
| smoker         | Smoking status                          |
| region         | Region of residence (US)                |
| charges        | Medical cost billed to insurance        |



##  Exploratory Data Analysis (EDA)

-  **Histogram** to visualize charge distribution  
-  **Boxplot** of charges by smoking status  
-  **Heatmap** to analyze correlations between features and charges  

EDA showed that **smoking**, **age**, and **bmi** are strong predictors of high medical costs.



##  Preprocessing

- Handled categorical data with `LabelEncoder` and `OneHotEncoder`
- Checked and confirmed no missing values
- Final dataset ready for regression modeling



##  Model Used

- **Linear Regression**
- **Train/Test Split**: 80/20

###  Model Evaluation

| Metric   | Value         |
|----------|---------------|
| MAE      | ~4181.1944    |
| RMSE     | ~5796.284     |
| R² Score | ~78%          |

The model provides strong baseline predictions. It can be extended with more features (like activity level, medical history, diet score) in the future.



##  Results Visualization

-  **Scatter Plot**: Actual vs Predicted charges
- Model shows good fit for the majority, but may overestimate a few extreme cases (e.g., smokers with high BMI)
