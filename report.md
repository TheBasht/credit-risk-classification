# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis is to check if a machine learning model can predict if a loan is healthy (`0`) or high-risk (`1`). This is important because it helps the company decide which loans to approve or deny.

The data had financial information like loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, and total debt. The main variable we wanted to predict was the `loan_status`, which is either `0` for healthy or `1` for high-risk.

We used a Logistic Regression model to do this prediction. The machine learning process included splitting the data into training and testing sets, training the model, and then testing it to see how good it is. After this, we checked its performance using accuracy, precision, and recall scores.

## Results

* **Machine Learning Model 1: Logistic Regression**
  * **Confusion Matrix:**  
    ```
    [[18655   110]
     [   36   583]]
    ```
    This shows that the model correctly predicted 18,655 healthy loans (`0`) and 583 high-risk loans (`1`). It made 110 mistakes predicting `0` and 36 mistakes predicting `1`.
  * **Classification Report:**
    ```
                  precision    recall  f1-score   support

               0       1.00      0.99      1.00     18765
               1       0.84      0.94      0.89       619

        accuracy                           0.99     19384
       macro avg       0.92      0.97      0.94     19384
    weighted avg       0.99      0.99      0.99     19384
    ```
    This shows the model is very good at predicting `0` (healthy loans) with almost perfect precision, recall, and F1 scores. For `1` (high-risk loans), the model has a lower precision (84%) but still good recall (94%) and F1-score (89%).

## Summary

The Logistic Regression model works well for predicting healthy loans (`0`), but it is not very strong for finding high-risk loans (`1`). If the company cares more about avoiding high-risk loans, this model might not be the best choice because it misses some of them.

However, if predicting healthy loans is more important, then this model can help a lot. It depends on what the company wants to focus on. Overall, I would recommend using this model but maybe improving it or combining it with other methods to catch more high-risk loans.
