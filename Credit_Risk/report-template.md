# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of this analysis is to develop a predictive model that can assist in assessing loan risks based on various borrower attributes or features. This could have practical applications in financial institutions or lending organizations for making informed decisions about loan approvals or risk management. The data is split into two main components: labels (y) and features (X). The labels represent the target variable, which in this case is the loan status (healthy or high-risk). The features encompass all other attributes or variables that might influence the loan status prediction: loan size, interest rate, income, debt to income ratio, number of accounts, deragatory marks and total debt.

The data is divided into training and testing sets using the train_test_split function. This splitting allows for model training on one portion of the data and evaluation on another, unseen portion. It helps assess how well the model generalizes to new, unseen data.

A logistic regression model is instantiated and trained using the training data. Logistic regression is a common choice for binary classification tasks, such as predicting loan statuses, where the outcome variable has two possible outcomes.

The trained model's performance is evaluated using the testing data. This evaluation involves generating a confusion matrix and printing a classification report. These metrics provide insights into how well the model is performing in terms of correctly predicting healthy loans (0) and high-risk loans (1).

Finally, there's a qualitative assessment of the model's performance. In this case, attention is drawn to the accuracy and performance metrics for both healthy and high-risk loans. This interpretation helps understand the model's strengths and weaknesses and guides potential improvements or further analyses.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

Model 1: Logistic Regression Model

Accuracy Score: 99%
Precision Score for Healthy Loans (0): 100%
Precision Score for High-Risk Loans (1): 85%
Recall Score for Healthy Loans (0): 100%
Recall Score for High-Risk Loans (1): 85%

Model 2: Decision Tree Classifier

Accuracy Score: 98%
Precision Score for Healthy Loans (0): 99%
Precision Score for High-Risk Loans (1): 85%
Recall Score for Healthy Loans (0): 99%
Recall Score for High-Risk Loans (1): 82%

Model 3: Random Forest Classifier

Accuracy Score: 99%
Precision Score for Healthy Loans (0): 99%
Precision Score for High-Risk Loans (1): 91%
Recall Score for Healthy Loans (0): 100%
Recall Score for High-Risk Loans (1): 85%

Model 4: Support Vector Machine (SVM) Classifier

Accuracy Score: 97%
Precision Score for Healthy Loans (0): 99%
Precision Score for High-Risk Loans (1): 82%
Recall Score for Healthy Loans (0): 98%
Recall Score for High-Risk Loans (1): 78%

Model 5: Gradient Boosting Classifier

Accuracy Score: 99%
Precision Score for Healthy Loans (0): 99%
Precision Score for High-Risk Loans (1): 93%
Recall Score for Healthy Loans (0): 100%
Recall Score for High-Risk Loans (1): 85%

## Summary

Considering the overall performance, especially in terms of accuracy, precision, and recall, the Logistic Regression Model appears to be the most suitable choice. It achieved the highest accuracy and demonstrated robust performance in predicting both healthy and high-risk loans. Moreover, logistic regression is relatively interpretable, making it easier to understand the model's decision-making process, which could be advantageous in a lending context where explainability is crucial.

However, it's important to note that the choice of model should also consider practical factors such as computational resources, scalability, and interpretability requirements. Therefore, it's recommended to further validate the logistic regression model's performance on unseen data and conduct sensitivity analyses to ensure its suitability for deployment in a real-world lending environment.
