# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of this analysis is to create a data model that predicts the credit of potential borrowers from peer-to-peer lending services

* Explain what financial information the data was on, and what you needed to predict.
The financial infromation was used to determine credit worthiness of potential borrowers.  The data provided included loan_size,interest_rate,borrower_income,debt_to_income,num_of_accounts,derogatory_marks,total_debt,loan_status.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
Value counts was used to determine how many loans of each.  The results found 75036 and 2500 loans initially.

* Describe the stages of the machine learning process you went through as part of this analysis.
Machine learning was used to make these predictions.  After reviewing the data, the loan_status column was set to the y variable. Next the DataFrame created stored all the columns except loan_status in the X variable. The train_test_split was used to split the data into training and testing variables that would be used to make the predictions through sklearn techniques.  RandomOverSampler was used to resample the data and that was used in the LogisticRegression. From both samples, I calculated accuracy score, confusion matrix, and classification report.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
The methods used from sklearn were balanced_accuracy_score, and confusion_matrix, classification_report and LogisticRegression.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    Balanced Accuracy Score: taking into account the sensitivity and specificity of the model, the balanced prediction accuracy was 95.2%
    Precision Score: 100% and 85% of predicted positives were correct for each loan type
    Recall Score: The model was 99% and 91% precise in measuring values of predictions made for each loan type

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    Balanced Accuracy Score: taking into account the sensitivity and specificity of the model, the balanced prediction accuracy was 99.5%
    Precision Score: 100% and 99% of predicted positives were correct for each loan type
    Recall Score: The model was 99% and 100% precise in measuring values of predictions made for each loan type

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
I would recommend using the model to predict the creditworthiness because of the accuracy in predicting the outcome for the repayment of the loan. 


