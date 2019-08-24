# analyticsVidhya-IndiaML-khanij
Solution and approach by Khanij for Analytics Viddhya India ML 2019 Challenge

# Approach:
We consider this as logistic regression classification problem. We do the following.

- Exploratory analysis
- One variable regression to understand the importance of a given variable.
- Model building considering the important variables from the above steps.
- Feature enginering(Iterative) to improve the f1-score.

## We are documenting the final results here, for quick reference
- We derive new variables , 'new_deliquency_score' and 'new_credit_score' which are used in the final model. 'new Deliqunecy score' indicates whether loan repayment pattern is improving or not. 'new_credit score' is average of borrower and co-borrower credit score(if applicable).
- Our final model consists of the following variables. (f1-score 31.52% on test data)
"interest_rate","debt_to_income_ratio", "new_cred_score","new_deliquency_score"


## Score for improvement
- SMOT resampling to address imbalanced data
- outlier analysis
- Standardising variables and rebuilding the model.
