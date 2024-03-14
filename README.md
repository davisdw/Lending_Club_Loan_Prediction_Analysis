# Lending_Tree_Loan_Prediction_Analysis



# Weighted Average Analysis
Based on the feature importances obtained from the predictive model, we can observe the following key findings:

issued_year (Issued Year): This feature has the highest importance score of 0.0321, indicating that the year in which the loan was issued is the most significant predictor of loan default according to the model. Newer loans might have different risk factors compared to older ones, which could influence default rates.

int_rate (Interest Rate): With an importance score of 0.0199, the interest rate charged on the loan is the second most important feature. This aligns with common intuition as higher interest rates typically correlate with higher risk for default.

dti (Debt-to-Income Ratio): The debt-to-income ratio has an importance score of 0.0129, indicating its moderate importance in predicting loan defaults. A higher DTI suggests that the borrower may have difficulty managing additional debt, increasing the risk of default.

annual_inc (Annual Income): This feature has an importance score of 0.0105, suggesting that the borrower's annual income plays a role in predicting loan defaults. Higher income levels may indicate greater financial stability and a lower likelihood of default.

installment (Loan Installment): With an importance score of 0.0100, the size of the loan installment also contributes to predicting loan defaults. Larger installments may strain the borrower's finances, increasing the risk of default.

fico_score (FICO Credit Score): The borrower's FICO credit score has an importance score of 0.0094, indicating its moderate importance in predicting defaults. Higher credit scores generally signify lower credit risk, so lower FICO scores might indicate a higher likelihood of default.

loan_amnt (Loan Amount): This feature has an importance score of 0.0085, suggesting that the size of the loan also plays a role in predicting defaults. Larger loan amounts may present higher risk, especially if coupled with other factors like high interest rates or low income.

delinq_2yrs (Number of Delinquencies in the Past 2 Years): Lastly, the number of delinquencies in the past 2 years has the lowest importance score of 0.0027. While still contributing to the model's predictions, it appears to have less impact compared to the other features.

Overall, the results indicate that several factors, including the year of loan issuance, interest rate, debt-to-income ratio, annual income, and loan installment size, are important predictors of loan defaults. These insights can be valuable for lenders in assessing credit risk and making informed decisions about loan approvals.


![image](https://github.com/davisdw/Lending_Tree_Loan_Prediction_Analysis/assets/140672220/d992dd17-a90d-427a-a6ad-312380487662)

