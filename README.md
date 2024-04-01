# Lending_Club_Loan_Prediction_Analysis



![image](https://github.com/davisdw/Lending_Tree_Loan_Prediction_Analysis/assets/140672220/d992dd17-a90d-427a-a6ad-312380487662)




int_rate (Interest Rate): With an importance score of 0.0199, the interest rate charged on the loan is the second most important feature. This aligns with common intuition as higher interest rates typically correlate with higher risk for default.

dti (Debt-to-Income Ratio): The debt-to-income ratio has an importance score of 0.0129, indicating its moderate importance in predicting loan defaults. A higher DTI suggests that the borrower may have difficulty managing additional debt, increasing the risk of default.

annual_inc (Annual Income): This feature has an importance score of 0.0105, suggesting that the borrower's annual income plays a role in predicting loan defaults. Higher income levels may indicate greater financial stability and a lower likelihood of default.

installment (Loan Installment): With an importance score of 0.0100, the size of the loan installment also contributes to predicting loan defaults. Larger installments may strain the borrower's finances, increasing the risk of default.

fico_score (FICO Credit Score): The borrower's FICO credit score has an importance score of 0.0094, indicating its moderate importance in predicting defaults. Higher credit scores generally signify lower credit risk, so lower FICO scores might indicate a higher likelihood of default.

loan_amnt (Loan Amount): This feature has an importance score of 0.0085, suggesting that the size of the loan also plays a role in predicting defaults. Larger loan amounts may present higher risk, especially if coupled with other factors like high interest rates or low income.

delinq_2yrs (Number of Delinquencies in the Past 2 Years): Lastly, the number of delinquencies in the past 2 years has the lowest importance score of 0.0027. While still contributing to the model's predictions, it appears to have less impact compared to the other features.





![bar_stacked_bad_loan_region](https://github.com/davisdw/Lending_Tree_Loan_Prediction_Analysis/assets/104311388/172b5f32-b606-4247-a384-63548923787e)


Taking closer look into the bad loans by region determines the following: 

Plot takes in account of percentage average of each of those bad loan types Late, Default, and Charged Off

North East showing increase percentage of bad loans which especially with high number of Default loans within that region

26% of Late Payment discovered in  South East
33% of Default loan from North East
25% of Charged Off Loan from South East

Now let’s take a deeper look by state


![map_plot_default_ratio](https://github.com/davisdw/Lending_Tree_Loan_Prediction_Analysis/assets/104311388/838202ab-2631-4510-8564-09a13b88d5a1)


In this third plot each state is calculated based on a Default Ratio ( bad_loan / and good_loan ).groupby(state).avg(  ) 

I’ve included the average interest loan for each state (int_rate)groupby(state).avg ( )

State with highest Default Ratio -> IN (Indiana) and IL(Illinois) are tied around .18 (with interest rates of IL with 19% and IN with 18%)

This indicated that the loan lending out bad loans  (%)  in those two states (IL 1.45% and ID 0.90% ) are very low (which chances of residents in either of those states are quite low)





![good_bad_loan_pie_bar](https://github.com/davisdw/Lending_Tree_Loan_Prediction_Analysis/assets/104311388/9dcd6c32-41bf-4053-bd77-02c70f4f6e42)



Breakdown of the loans based on the conditions of the loan status 

Bad loan consists of compilation of Late payments 31 - 120 Days, Default and Charged Off

Good loan which is current, paid off, and even grace period (16-30 days of late payment)

Now let’s take closer look at the bad data




![confuse_matrix](https://github.com/davisdw/Lending_Tree_Loan_Prediction_Analysis/assets/104311388/f67bf527-1a36-4942-950d-cc8d7448a25f)



Took it further and use confusion matrix to determine how the model made it’s prediction 

To test how accurate Lending Club makes their loan decisions, used logistic regression model 

S/N: data has to be numeric and free of any Null values 

Splitted the data into features and labels using train_test_split 

Trained the model with logistic regression which was able to achieve my desired results before running test 

Test the model with prediction and returned score of .88


# Weighted Average Analysis



![feature_importance_plot](https://github.com/davisdw/Lending_Tree_Loan_Prediction_Analysis/assets/104311388/bf8acf48-0c3a-412b-96a7-70c42b90addd)



Based on the feature importances obtained from the predictive model, we can observe the following key findings:

issued_year (Issued Year): This feature has the highest importance score of 0.0321, indicating that the year in which the loan was issued is the most significant predictor of loan default according to the model. Newer loans might have different risk factors compared to older ones, which could influence default rates.


Overall, the results indicate that several factors, including the year of loan issuance, interest rate, debt-to-income ratio, annual income, and loan installment size, are important predictors of loan defaults. These insights can be valuable for lenders in assessing credit risk and making informed decisions about loan approvals.


