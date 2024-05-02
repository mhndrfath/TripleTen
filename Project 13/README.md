# Taxi Order Model with Time Series

## Project Description
At Sweet Lift, a taxi company, the task is to develop a model for predicting the number of taxi orders at airports for the next hour using historical data. The goal is to attract more drivers during peak hours by accurately forecasting demand.

The RMSE metric on the test set should not be more than 48.

## Data Description
Dataset is stored in files `taxi.csv`

The order amount can be found in the column `num_orders`.

## Methodology
- Data Overview
- Data Pre-processing
  - Handle duplicate and missing values
  - Resample
  - Features Engineering
- Model Training and Validation
- Model Testing

## Result
1. **Data Preparation**
- Data Description
  - Dataset contains 2 columns (datetime & num_orders) with 26.496 rows
  - The duplicates or missing value are not found
  - The 'datetime' column will be convert to timestamp format to simplify analyze
- Duplicate & Missing Value
  - Dataset contains 2 columns (datetime & num_orders) with 26.496 rows
  - The duplicates or missing value are not found
  - The 'datetime' column will be convert to timestamp format to simplify analyze
- Data Resample & Features Engineering
  - New dataset contain around 16% from old dataset after resampling which is 4416 rows
  - New columns such as month, date, and hour are added for knowing when the taxi order occurred
  - 3 lag Features and mean average of 5 also added to gain some information about previous values and 'smooth' the distribution of data


2. **Data Analysis**
- The first and second paragraphs gives information about non-stationary distribution of taxi orders in 6 months period
  - The trend graphic shows the taxi orders in the end of period increase about 3 times from the beginning of period
  - There is a cycle in seasonal graphic that shows the highest order for a taxi happen around midnight to dawn, while the least time happen at the beginning of sunrise

3. **Model Training & Validation**
- The result for each model for the RMSE is quite similar, which only range from 40-43
- Linear regression has the best result for data training and validation, that generate the RMSE at around 40
- The differences are not too different which will be continued at the testing stage using all models to be sure

***Model Testing & Main Conclusion***
- Linear Regression still the best model for this prediction which has result of RMSE at around 53, while the other model range from 58-61 for the RMSE.
- Still the RMSE can't reach under 48, besides not using the validation data

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
