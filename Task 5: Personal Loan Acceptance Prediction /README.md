#  Smart Campaign Analyzer — Predicting Personal Loan Acceptance

This project is part of my **Data Science & Analytics Internship** at **DevelopersHub Corporation**.  
The aim is to predict which bank customers are most likely to accept a personal loan offer using historical campaign data.

---

##  Objective

To build a classification model that helps the bank's marketing team target customers more likely to accept personal loan offers — saving time, budget, and increasing conversion success.



##  Dataset

- **File:** `bank-marketing.csv`
- **Target Variable:** `deposit` (yes = accepted, no = rejected)
- **Rows:** ~11,000
- **Features:** Age, Job, Marital Status, Education, Loan, Housing, Contact Duration, Month, and more.



##  Data Preparation

- Cleaned target column `deposit` by standardizing and mapping:
  - `'yes'` → `1`, `'no'` → `0`
- Encoded all categorical columns using `LabelEncoder`
- Verified dataset completeness and consistency



##  Exploratory Data Analysis (EDA)

-  **Countplot** to visualize acceptance ratio
-  **Boxplot** to analyze age vs acceptance
-  **Duration** found as the most influential feature (longer calls = more conversions)
-  **Heatmap** revealed strong correlations with `duration`, `month`, and `campaign`



##  Model Used

- **Algorithm:** Decision Tree Classifier  
- **Train/Test Split:** 80/20  
- **Max Depth:** 5



##  Model Evaluation

| Metric        | Score |
|---------------|-------|
| Accuracy      | 81%   |
| Precision (0) | 86%   |
| Recall (1)    | 87%   |
| F1 Score      | 80–81% |

The model balanced recall and precision well, making it useful for predicting both acceptance and rejection scenarios.



##  Feature Importance

Top features influencing customer decisions:
1. `duration` (length of call)
2. `contact` (contact method)
3. `month` (month of contact)
4. `age`
5. `campaign` (number of contacts)
