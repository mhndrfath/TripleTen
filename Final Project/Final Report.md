**Introduction**

This project aims to predict when telecom customers might stop using the company's services, which is called "customer churn." To do this, they're using data like customer information, account details, and usage patterns. The goal is to make a model that can find customers who might leave and provide useful insights to help the business keep them.

**Pre-processing Data**

The initial task in this project was data preprocessing. This involved merging contract, personal, and service data, dealing with missing values, removing unnecessary variables, and converting categorical variables into nominal ones. Then, the data was divided into an 80% training set and a 20% testing set for model development and evaluation.

**Exploratory Data Analysis (EDA)**

After preparing the data, we conducted exploratory data analysis (EDA) to better understand it. During EDA, we looked for patterns and relationships between different variables and customer churn. Here are some insights from our analysis:

1. Customers with shorter-term contracts are more prone to leaving the company.
2. Compared to customers with long-term contracts, those with monthly contracts are more likely to churn.
3. Customers who use data security services without having internet access are more likely to churn.
4. Customers with low monthly charges are at a higher risk of leaving.
5. Senior customers are more inclined to leave the company.
6. Customers with long-term contracts are more common among those who have children and partners.

**Model Training and Evaluation**

In our effort to predict customer churn, we employed a range of machine learning models. These included Logistic Regression, KNearest Neighbor, Decision Tree, Random Forest, Gradient Boosting with CatBoost and XGBoost, as well as an Artificial Neural Network (ANN) implemented with Keras.

To evaluate these models, we used the ROC-AUC score. Notably, the ANN model outperformed the others, achieving an impressive ROC-AUC score of 85% on the test dataset. The remaining models demonstrated ROC-AUC scores ranging from 70% to 80%.

**Important Feature**:

We also examined the significance of different features in predicting churn. The top five crucial factors include contract duration, monthly fees, total charges, the number of months a customer has been with the company totalmonths, payment method, and internet service. By focusing on these aspects, the business can effectively reduce churn.

**Result**

The table below presents the ROC-AUC scores for each model on both the training and test sets:

- Logistic Regression produces 75% on test set.
- K Nearest Neighbor produces 71% on the test set.
- Decision Tree produces 75% on the test set.
- Random Forest produces 77% on test set.
- CatBoost produces 76% on the test set.
- XGBoost produces 73% on the test set.
- Artificial Neural Network produces 85% on the test set.

**Difficulty**

Selecting an appropriate model for training the data presented a challenge in this project. This was particularly evident in the algorithms we selected, where some exhibited the issue of overfitting.

**Conclusion**

This project showcases the practicality of using machine learning models to predict customer churn in the telecom sector. The Artificial Neural Network model stood out with an impressive 85% ROC-AUC score, demonstrating its superior performance. By delving into feature importance, businesses can discern the pivotal factors for churn prediction and proactively retain customers. In essence, this research underscores the potential of data science and machine learning in addressing business dilemmas, such as customer turnover.

**Recommendation**


To reduce customer attrition rates, telecom business Interconnect can consider the following recommendations based on predictive model insights:

1. *Personalized Offers*: Tailor discounts and promotions to customer preferences and usage data to foster loyalty.

2. *Enhanced Customer Support*: Prioritize quick resolution of customer issues to boost satisfaction and reduce churn.

3. *Simplified Payments*: Improve user-friendliness and offer flexible payment options to save customers time and strengthen loyalty.

4. *Regular Satisfaction Surveys*: Continuously track customer satisfaction through surveys and feedback channels to identify improvement areas.

5. *Loyalty Programs*: Implement loyalty programs to reward customer loyalty, encouraging them to stay with the telecom service.

6. *Data Analysis*: Analyze churn data to identify trends and root causes, enabling more effective issue resolution and retention strategies.

7. *Effective Communication*: Keep customers informed about new products and services through newsletters, emails, and SMS, while also addressing their concerns promptly.
