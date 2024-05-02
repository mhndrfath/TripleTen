# Insurance Company Task for Data Masking

## Project Description
Sure Tomorrow, an insurance company, seeks to address various challenges through machine learning, and the task is to evaluate the feasibility of these solutions.

- Task 1 involves identifying clients similar to certain criteria to facilitate targeted marketing efforts.
- Task 2 focuses on predicting whether a new client is likely to file an insurance claim and assessing if the model predictions outperform those of a dummy model.
- Task 3 aims to predict the size of an insurance claim a new client might receive using a linear regression model.
- Task 4 emphasizes protecting clients' personal data without compromising the effectiveness of the predictive model. This entails developing data transformation algorithms to prevent misuse of personal information, known as data hiding or obfuscation. 

It's crucial to ensure that data protection procedures are implemented without compromising the model's quality. The objective is not to select the best model but to demonstrate the accuracy and effectiveness of the algorithm in safeguarding personal data while maintaining model performance.

## Data Description
Dataset is stored in files `insurance_ud.csv`
- `Features`: gender, age, salary, and number of family members of the insured person.
- `Target`: the number of claims received by insured people during the last five years.

## Methodology
- Data Overview
- Explorative Data Analysis
- Task
  - Task 1 (Similar Clients)
  - Task 2 (Is the client likely to receive an insurance claim)
  - Task 3 (Regression)
  - Task 4 (Data Obfuscation)
- Proof that Data Obfuscation can work with Linear Regression
- Linear Regression Test with Data Fuzzing

## Result
- When checking the data, data pre-processing is carried out, where data types are changed in 2 columns, namely the 'age' and 'income' columns
- In task 1, analysis has been carried out to display client groupings to make calculations easier with the kNN model
- The distance used also uses 3 different models so that you can see the picture in the kNN model
- Euclidean and Manhattan distances look almost the same, but the accuracy of the results is still at Euclidean distance, considering that this distance ignores *block distance*
- In task 2, scaling is carried out on the data to calculate the F1 score
- A very good F1 score was produced on the data that had been scaled, namely 0.93, which was very far from the result compared to the data before scaling, namely 0.19
- This good result occurs because when scaling, the data uses a certain specific scale which is very good for the kNN model
- In task 3, RMSE and R2 are calculated in the linear regression model
- The results obtained use original data and data that has been scaled, where the results are not different at all, namely RMSE is at 0.34 and R2 at 0.66, this happens because linear regression is not too affected by scaling
- In task 4, data obfuscation is carried out, which aims to maintain the privacy of the data so that it is only known by the party concerned
- Calculations were also carried out on a linear regression model using data obfuscation, where the results were no different from using original data, this happened because the form of the data was the same, only disguised. Therefore, data blurring will not affect the Linear Regression calculations

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
