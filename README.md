# Data-Science-Portfolio-
This portfolio showcases a collection of Data Science and Data Analysis projects I have undertaken for personal growth and passion-driven learning. It highlights my achievements and technical skills with regular updates to reflect my ongoing journey and progress in the field.
- Email:rethabilethuto3@gmail.com 
- LinkedIn:https://www.linkedin.com/in/rethabile-kgolobe-b82121265?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app
# Projects

## Machine learning: [Loan Approval Prediction](LoanApprovalPrediction.ipynb)

1. **Loan Approval Prediction:**
   
## Overview: 

- Loans are one of the significant sources of income for banks and play a critical role in the economy and in individuals managing expenses, purchasing luxuries, etc. However, banks must examine many factors to assess whether the candidate is granted a loan. Since there are many features, banks can automate this process using machine learning tools to reduce the time taken for decision-making.
      
## Objective: 

-To develop a robust machine learning tool that will determine whether a loan application should be accepted based on the applicant's features, such as marital status, education level, income, etc.
      
## Dataset: 
- Source: [https://drive.google.com/file/d/1LIvIdqdHDFEGnfzIgEh4L6GFirzsE3US/view]
     
## Features Description:

| Feature             | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `Loan`             | A unique identifier for each loan.                                          |
| `Gender`           | Gender of the applicant (Male/Female).                                      |
| `Married`          | Marital status of the applicant (Yes/No).                                   |
| `Dependents`       | Number of dependents of the applicant.                                      |
| `Education`        | Educational status of the applicant (Graduate/Not Graduate).               |
| `Self_Employed`    | Indicates whether the applicant is self-employed (Yes/No).                 |
| `ApplicantIncome`  | Income of the applicant.                                                   |
| `CoapplicantIncome`| Income of the co-applicant.                                                |
| `LoanAmount`       | Loan amount (in thousands).                                                |
| `Loan_Amount_Term` | Loan terms (in months).                                                    |
| `Credit_History`   | Credit history representing the repayment record of debts.                 |
| `Property_Area`    | Type of property area (Rural/Urban/Semi-urban).                            |
| `Loan_Status`      | Loan approval status (`Y` - Approved, `N` - Not Approved).

## Methods:

1. **Data Preprocessing**:
   - Handling missing values
   - Handling Outliers
   - Feature Engineering
2. **Models Development**:
   - Random Forest
   - Gradient Boosting
   - XG Boosting
3. **Evaluation**:
   - Model performance was evaluated using accuracy, precision, recall, and F1 score.
4. **Hyperparameter tuning**:
   - The best-performing model, Random Forest, was tuned to optimize its performance.
   - The tuning process utilizes Grid search to search for the best parameters combined with cross-validation.
     
## Results
- Random Forest performed well compared to the other two models, followed by XG Boosting with 0.8698 accuracy.
- Hyperparameter tuning was performed on Random forest to improve its accuracy from 0.8698 to 0.8835.
