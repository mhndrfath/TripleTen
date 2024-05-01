# Prediction of Bank Customer Models with Machine Learning

## Project Description
At Bank Beta, a significant decline in the number of customers has been observed over time, prompting officials to prioritize retaining existing loyal customers over acquiring new ones.

The task at hand is to predict whether a customer is likely to leave the bank soon. Data on the past behavior of clients and the history of contract terminations with the bank are available for analysis.

The objective is to create a model with the maximum possible F1 score. A minimum F1 score of 0.59 for the test dataset is required to pass the review. The F1 value for the test set will be evaluated to ensure it meets this criterion.

Additionally, the AUC-ROC metric will be measured and compared to the F1 score to provide a comprehensive evaluation of the model's performance.

## Data Description
Dataset is stored in files `churn.csv`

Features:
- `RowNumber` — data string index
- `CustomerId` — Customer ID
- `Surname` — last name
- `CreditScore` — credit score
- `Geography` — country of residence
- `Gender` — gender
- `Age` — age
- `Tenure` — maturity period for customer fixed deposits (years)
- `Balance` — account balance
- `NumOfProducts` — number of bank products used by customers
- `HasCrCard` — whether the customer has a credit card
- `IsActiveMember` — customer activity level
- `EstimatedSalary` — estimated salary

Targets:
- `Exited` — whether the customer has stopped

## Methodology
- Data Overview
- Data Pre-Processing
  - Handling lower case and unused column
  - Handling missing value
  - Encoding column
- Modelling Preparation
  - Balancing Data
  - Devide dataset into train, valid, and test data
  - Scaling Features
- Modelling
  - With default hyperparameter
  - With tuning hyperparameter
- Balancing Data Modelling
  - Class weight adjustment
  - Upsampling
  - Downsampling

## Result
- Performing data balance greatly affects the value of the F1 score and also the AUC-ROC value
- In this analysis, data balance using an upsample approach, which multiplies minor data, produces the best F1 score and AUC-ROC values
- The model with the best results is the Random Forest model using hyperparameter tuning
- The F1 Score results obtained were 0.609 on validation data and 0.613 on test data
- The resulting AUC-ROC results are 0.766 on validation data and 0.759 on test data
- Selection of the best model based on the F1 Score and AUC-ROC results, not only a high number but also the difference between the validation and test values, so that it does not cause excessive overfitting or underfitting, as can be seen from the test value being slightly better than the validation value

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
