# Prediction of Car Price with Numerical Method

## Project Description
At Rusty Bargain, a used car buying and selling company, the task is to develop an application that provides users with the market value of their cars. The available data includes historical data, vehicle technical specifications, vehicle model versions, and vehicle prices. The objective is to create a model capable of determining the market value of a car.

Rusty Bargain is interested in:
- Prediction quality
- Prediction speed
- Time required to train the model

## Data Description
Data Features :
- `DateCrawled` — date of profile that was downloaded from database
- `VehicleType` — vehicle body type
- `RegistrationYear` — year of registration
- `Gearbox` — transmission type
- `Power` — power (hp)
- `Model` — vehicle model
- `Mileage` — mileage (in km based on regional)
- `RegistrationMonth` — month of registration
- `FuelType` — fuel type
- `Brand` — vehicle brand
- `NotRepaired` — repaired or not yet
- `DateCreated` — date of new profile
- `NumberOfPictures` — picture of vehicle
- `PostalCode` — postal code (owner)
- `LastSeen` — date of last activity (user)

Target
- `Price` — vehicle price (in Euro)

## Methodology
- Data Overview
- Data Pre-Processing
  - Lowercase and discharged columns
  - Handling anomaly value, duplicate and missing value
- Explorative Data Analysis
  - Numerical Data
  - Categorical Data
- Data Encoding for Modelling
  - One-hot encoding
  - Ordinal encoding
  - Split dataset into train, valid, and test data
- Model Training and Analysis

## Result
**Data Encoding**
- New dataset of OHE contained 303 new columns and 5 rows
- The categoric data were chose to transform into numerical data in Ordinal Encoding

**Model Training and Analysing**
- Random Forest need 4 minutes in total to train the model, set the range of parameter depth and estimator still not generate the best result among the other model.
- XGBoost take up to 12 min to train the model for just a few parameters, considering the data used is OHE which has more than 300 columns.
- LightGBM with range of parameters in depth and num_leaves takes about 1 minutes to train the model and the result almost the same with Random Forest for the best result
- CatBoost has least time taken to train the model which is 56 seconds, considering the dataset has a number of categorical data and CatBoost has the advantage for that.

***Main Conclusion***
- The best result for overall with the least time to train the model and the best RMSE produced by LightGBM that takes 1 minutes 21 seconds for the train and valid data, while takes about 3 seconds for test data. The result of RMSE was the best among the other model which is only 1644 for test data with parameter of depth = 5 and num_leaves = 40

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
