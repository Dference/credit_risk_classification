# credit_risk_classification

## Risky Business
For this Challenge, I used various techniques to train and evaluate a model based on loan risk. I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. To execute the challenge, I followed the following process: 

-Split the Data into Training and Testing Sets

-Created a Logistic Regression Model with the Original Data

-Wrote the upcoming Credit Risk Analysis Report

## Credit Risk Analysis Report

-The overall purpose of the analysis was to identify loans risk potential and the borrowers credit impact on potential.

-The financial information was located on a lending data csv file, which I extracted using Pandas, to predict the possible health of the borrowers loan.

-The variables I used to do this were broken down into x for the features and y for the labels.  I extracted the column loan_status from the DataFrame and assigned it to the variable y. This variable y will be the target variable, which I wanted to predict. I then created a new DataFrane for the variable x and dropped the loan_status column, so contained all the columns except loan_status, which were my feature variables used for making predictions.

-For the machine learning process, I followed the following steps other than listed above: Split the data into training and testing datasets by using train_test_split. 
Fit a logistic regression model by using the training data (X_train and y_train).
Saved the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model.
Evaluated the model’s performance by generating a confusion matrix and classification report.

## Results
                precision   recall   f1-score  support

           0       1.00      1.00      1.00     18759
           1       0.87      0.89      0.88       625

    accuracy                           0.99     19384
    macro avg        0.94     0.94     0.94     19384
    weighted avg     0.99     0.99     0.99     19384
   
## Summary

The overall performance of both turned out to be very good, with high precision and recall scores, but the performance for healthy loans was much better than the at risk loans. The higher recall for the at risk loans shows that the model performs well, but the lower precision score shows that it still does err when selecting loans, with the f1-score showing overall success with room to improve. The performance is crucial when trying to predict the loans risks, though with higher healthy scores showing better results, that should be taken as a given as that is the foundation for why the loans were considered at risk to begin with on the reverse side.
