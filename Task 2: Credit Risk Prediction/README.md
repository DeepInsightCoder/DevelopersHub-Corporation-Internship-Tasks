#  Loan Approval Assistant AI — Credit Risk Prediction

This project is part of my **Data Science & Analytics Internship** at **DevelopersHub Corporation**.  
We use a machine learning model to predict whether a loan application is likely to be approved or rejected, based on applicant financial and demographic information.



##  Objective

To build a smart loan approval prediction system using a real-world dataset.  
This system can assist financial institutions in identifying low-risk loan applicants.



##  Dataset Used

- **Training Data:** `train_u6lujuX_CVtuZ9i.csv`
- **Test Data:** `test_Y3wMUE5_7gLdaTN.csv`
- Source: [Kaggle Loan Prediction Problem Dataset](https://www.kaggle.com/competitions/loan-prediction-problem)



##  Key Features Used

- Gender, Marital Status, Education
- Employment type
- Applicant & Coapplicant income
- Loan amount & term
- Credit history
- Property area

---

## 📊 EDA Highlights

- 📌 **Pie chart** to show approval vs rejection rates  
- 💸 **Violin plots** to compare income against approval status  
- 🧮 **KDE plots** to visualize loan amount distributions  
- All plots created using `matplotlib` and `seaborn`

---

##  Data Preprocessing

- Handled missing values using median/mode imputation  
- Label Encoded categorical features (`Gender`, `Married`, `Education`, etc.)  
- Dropped irrelevant columns like `Loan_ID` before modeling



##  Model Used

- **Algorithm:** Logistic Regression  
- **Train/Test Split:** 80/20  
- **Accuracy Achieved:** `78.86%`

###  Evaluation

| Metric         | Score      |
|----------------|------------|
| Accuracy       | 78.86%     |
| Precision (0)  | 95%        |
| Recall (1)     | 99%        |
| F1-score (1)   | 86%        |

Model is **highly sensitive to loan approvals**, ensuring most eligible applicants are approved — useful in real-world banking scenarios.
