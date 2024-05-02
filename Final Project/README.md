# Telecom Client Churn Model

## Project Description
The telecom operator Interconnect aims to forecast client churn to proactively address potential departures by offering promotional codes and special plan options. The marketing team has gathered personal data from their clientele, including information about their plans and contracts.

Interconnect primarily offers two types of services: 
- landline communication, where the telephone can be connected to multiple lines simultaneously
- Internet services, which can be set up via DSL or fiber optic cable.

Additionally, Interconnect provides supplementary services such as internet security with 
- Antivirus software (DeviceProtection) and a malicious website blocker (OnlineSecurity)
- Dedicated technical support (TechSupport)
- Cloud file storage and data backup (OnlineBackup)
- TV streaming (StreamingTV) and access to a movie directory (StreamingMovies).

Clients have the option to choose between monthly payments or signing 1- or 2-year contracts, and they can utilize various payment methods, receiving electronic invoices after transactions.

## Data Description
Dataset are stored in files:
- `contract.csv` — contract information
- `personal.csv` — the client's personal data
- `internet.csv` — information about Internet services
- `phone.csv` — information about telephone services

In each file, the column `customerID` contains a unique code assigned to each client.
The contract information is valid as of February 1, 2020.

## Methodology
- Data Overview
- Data Pre-Processing
  - Feature Engineering
  - Dataset Merger
  - Handling duplicate and missing values
- Explorative Data Analysis
  - Numeric data distribution
  - Categoric data distribution
- Modelling
  - Features Engineering (Machine Learning and CatBoost)
- Model Training
  - Basic parameter for all models
  - Model Evaluation
  - Logistic Regression
  - K Nearest Neighbor
  - Decision Tree
  - Random Forest
  - CatBoost
  - XGBoost
  - Artificial Neural Network

## Result
We have trained the data using several models. Some models happen to have overfitting even though we have used cross-validation to train the train set.

Here is summary of ROC-AUC score:

- Logistic Regression, 88% on train set using cross-validation, 75% on test set.
- K Nearest Neighbor, 89% on the train set using cross-validation, 71% on the test set.
- Decision Tree, 85% on the train set using cross-validation, 75% on the test set.
- Random Forest, 88% on train set using cross-validation, 77% on test set.
- CatBoost, 88% on the train set using cross-validation, 76% on the test set.
- XGBoost, 92% on the train set using cross-validation, 73% on the test set.
- Artificial Neural Network, 84% on the train set using cross-validation, 85% on the test set.

The best model in this project is the Artificial Neural Network model and also a short time to train this model.

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
