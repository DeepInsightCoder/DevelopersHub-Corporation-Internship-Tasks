## Loan Default Risk with Business Cost Optimization

### Objective

Predict the likelihood of loan default using logistic regression and evaluate cost-based decisions by adjusting prediction thresholds.

### Dataset

**Home Credit Risk Dataset**
Key columns:
`person_age`, `person_income`, `person_home_ownership`, `person_emp_length`, `loan_intent`, `loan_grade`, `loan_amnt`, `loan_int_rate`, `loan_status`, `cb_person_default_on_file`, `cb_person_cred_hist_length`

### Steps Performed

1. **Data Preprocessing**

   * Handled missing values
   * Encoded categorical features using One-Hot Encoding
   * Feature scaling with `StandardScaler`

2. **Model Training**

   * Applied **Logistic Regression** as the primary model
   * Evaluated using **accuracy**, **classification report**, and **confusion matrix**

3. **Visualization**

   * Feature importance (coefficients)
   * Class distribution and prediction heatmaps

4. **Cost-Benefit Analysis**

   * Adjusted classification threshold (e.g., 0.3 instead of 0.5)
   * Evaluated:

     * False Positives (FP): Loans given to defaulters
     * False Negatives (FN): Safe borrowers rejected
   * Custom business cost formula:

     ```
     Cost = FP * $10,000 (loss per default) + FN * $2,000 (lost revenue)
     ```

5. **Business Impact Insight**

   * Lower threshold reduced total loss from misclassification
   * Helped bank optimize loan approval strategy

### Results

* Custom threshold of **0.3** reduced business cost to **\$6,326,000**
* Demonstrated how model tuning directly impacts business profit/loss

### Skills Gained

* Logistic Regression for Risk Modeling
* Threshold tuning & probability prediction
* Business-driven decision-making
* Cost-Benefit Visualization
