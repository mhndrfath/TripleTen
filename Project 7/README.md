# Telecoms Plan with Machine Learning (Analyze Consumer Behavior and Recommend Megaline Packages)

## Project Description
At Megaline cellular operator, dissatisfaction arises due to a significant number of customers still using old packages. The company aims to address this issue by developing a model capable of analyzing consumer behavior and recommending one of Megaline's two new plans: Smart or Ultra.

Access to behavioral data of customers who have transitioned to the latest packages is available, as obtained from the Statistical Data Analysis course project. In this classification task, the objective is to develop a model that accurately selects packages.

Having completed the data pre-processing step, the project progresses to the model building stage. The goal is to develop a model with the highest possible accuracy, with a threshold set at 0.75 for the accuracy level. The model's accuracy metrics will be assessed using the test dataset.

## Data Description
Dataset is stored in files `users_behavior.csv`

Column Description
- `сalls` — number of calls
- `minutes` — total call duration in minutes
- `messages` — number of text messages
- `mb_used` — internet usage traffic in MB units
- `is_ultra` — plans for the current month (Ultra - 1, Smart - 0)

## Methodology
- Dataset Overview
- Modelling Preparation
  - Devide data into train, valid, and test data
- Modelling
  - With hyperparamater
  - Without Hyperparameter

## Result
Without Hyperparameter :
- The highest accuracy is found in the Random Forest model, where according to theory this model produces the highest accuracy compared to other models
- There is no overfitting or underfitting in the three models, because there is no significant difference between the accuracy produced by validation data and test data

With Hyperparameter :
- For hyperparameter depth in the Decision Tree and Random Forest models, the highest accuracy is in the Random Forest model where the difference is quite large, around 3%
- The Random Forest model has an accuracy of up to 80% using hyperparameter depth and n_estimator, which makes this model very suitable for predicting the right packet

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
