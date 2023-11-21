# Module 12 Report Template

## Overview of the Analysis

The purpse of the analysis was to predict credit risk. I used the lending_data.csv data which consisted of the loan size, interest rate, borrower income, debt to income, num of accounts, derogatory marks, total debt, and loan status. The data had 77,536 loans and there were 75,036 healthy loans and 2500 high risk loans.  

During the analysis, LogisticRegression was used with the oringal data set. I fit the model by using the training data (X_train and y_train) and saved the predictions for the testing data using X_test and the fitted model.  I evaluated the model by creating a confusion matrix and a classifiction report.  Then, RandomOverSampler was used with resampled data. Again, I fit the model this time using (X_res and y_res) and saved the predictions usig X_test and the fitted resample model. Lastly, ran a confustion matrix and classification report to see model was the most accurate.  

## Results

* Machine Learning Model 1:
- Balanced Accuracy: .95
- Precision Healthy Loans: 1.00
- Precision High Risk Loans: .85
- Recall Healthy Loans: .99
- Recall High Risk Loans: .91


* Machine Learning Model 2:
- Balanced Accuracy: .99
- Precision Healthy Loans: 1.00
- Precision High Risk Loans: .84
- Recall Healthy Loans: .99
- Recall High Risk Loans: .99

## Summary

The recommendation on the model to use would be Machine Learning Model 2. The precision is about the same for both models and both are accuarate at predicting healthy loans.  However, Machine Learning Model 2 has a better overall accuracy and higher recall for high risk loans. This helps tp predict less high risk loans which would be more important to the lender to ensure the borrowers creditworthiness.