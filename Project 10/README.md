# Gold Extraction Model

## Project Description
Zyfra is tasked with developing a machine learning model prototype capable of predicting the amount of gold extracted or obtained from gold ore. The company, specializing in developing efficient solutions for heavy industry, has access to data concerning the gold ore extraction and refining process. It is hoped that in the future, this model will aid in creating a more efficient production process and in eliminating parameters that do not produce profits.

## Data Description
Dataset are stored in rar files:
- `gold_recovery_full.csv`
- `gold_recovery_train.csv`
- `gold_recovery_test.csv`

Technological Process :
- `Rougher feed` — raw material for the flotation process
- `Rougher additions` (or reagent additions) — reagents for flotation: Xanthate, Sulphate, Depressant
- `Xanthate` — flotation activator or activator
- `Sulphate` — sodium sulfide, specifically for this process
- `Depressant` — sodium silicate
- `Rougher process` — flotation
- `Rougher tails` — product residue
- `Float banks` — flotation units
- `Cleaner process` — purification
- `Rougher Au` — a coarser gold concentrate
- `Final Au` — final gold concentrate
- Parameters of the Available Stages
- `air amount` — air volume
- `fluid levels`
- `feed size` — the size of the feed particles
- `feed rate`

Feature Naming :

[stage].[parameter_type].[parameter_name]

Example: rougher.input.feed_ag

Possible values for [stage]:
- `rougher — flotation
- `primary_cleaner — first cleanup
- `secondary_cleaner — secondary cleaning
- `final — final characteristic

Possible values for [parameter_type]:
- `input` — raw material parameters
- `output` — product parameters
- `state` — parameters indicating the characteristics of the current stage
- `calculation` — calculation of characteristics

## Methodology
- Data Overview
- Data Pre-Processing
  - MAE checking
  - Feauture analysis
  - Missing values checking
- Data Analysis
  - Metal concentration progress
  - Comparison of particle distribution
  - Total concentration of all substances
  - Handle missing values
- Modelling
  - Function for sMAPE (symmetric mean absolute percentage error)
  - Model evaluation with cross validation

## Result
- Columns used in both data, both training data and testing data, must have the same number, same column names, and have no missing values
- Missing values in the columns in both data can be replaced by any number or by the median depending on needs
- It is also very important to remove outliers to make it easier and to get results that match reality during the analysis and modeling process
- In the calculation to find the rough concentrate value, it was found that the calculated value and the actual value were not much different, it could be said that the resulting error was very small, where the number obtained was 9.303415616264301e-15
- The process of producing concentrate values for several types of metal produces different graphs
- The changes in particles used in the training data and testing data show no different graphs (after removing outlier values), so that the results obtained in the next step can be said to be safe
- By taking into account the target scale and predictions, the best model used to calculate sMAPE is the Random Forest Regression model with the conditions, depth=4 n_estimator=30
- The results obtained in the regression are worth 10.18966809276858 in the final prediction of the testing data

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
