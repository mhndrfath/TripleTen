# Prediction of New Locations of Oill Well with Machine Learning Model

## Project Description
At OilyGiant, an oil mining company, the task is to find a suitable location for digging a new oil well. The process involves several steps:

1. Collecting parameters for building oil wells in selected regions, including oil quality and volume of oil reserves.
2. Developing a model capable of predicting the volume of oil reserves in new wells.
3. Choosing the oil well with the highest estimated value based on the model predictions.
4. Selecting the area with the highest total profit for the chosen oil well.

Oil sample data from three regions is available, providing information on the parameters of each oil well in the area. The goal is to create a model to assist in selecting regions with the highest profit margins. Additionally, potential profits and risks will be analyzed using bootstrapping techniques.

## Data Description
Dataset are stored in files:
- `geo_data_0.csv`
- `geo_data_1.csv`
- `geo_data_2.csv`

Column Description:
- `id` — Unique ID of the oil well
- `f0, f1, f2` — three point features (the specific meaning is not important, but the features themselves are significant)
- `product` — volume of oil reserves in the well (thousands of barrels).

Condition:

- Only linear regression is suitable for model training (the rest are inadequate for prediction).
- When exploring the area, a study of 500 points was carried out by selecting the 200 best points for profit calculations.
- The budget to develop 200 oil wells is 100 million USD.
- One barrel of raw materials generates 4.5 USD in revenue. Income from one unit of product is 4,500 dollars (volume of oil reserves in thousands of barrels).
- After evaluating the risks, stick to only areas with a risk of loss lower than 2.5%. From the list of regions that meet the criteria, select the region with the highest average profit.

This data is artificial: contract details and well characteristics are not shown.

## Methodology
- Data Overview
- Modelling
  - Separate train and test data
  - Mean and RMSE calculation
- Basic Profit Calculation
- Modelling for Profit Calculation
- Profit and Risk Calculation

## Result
Profit Calculation :
- Region 0 gets the biggest advantage compared to the others from the target value and final value (prediction)
- In calculating the target value, region 2 has quite a big difference from the proper value, where the difference reaches approximately 10,000,000, where the difference in other regions is around 6,000,000 in region 0 and 700,000 in region 1
- Region 0 is a region that can be considered for further development because it produces quite high profits, followed by region 2 and region 1

Calculating the distribution of profits and risks is very necessary, in order to maximize profits for the company, therefore the following results are obtained:

- For region 0 1 2, the average profit value is almost the same as the bootstrap calculation and the 95% confidence interval, the average profit obtained is around 2.8 million dollars
- The resulting risk is the same for all three regions, at 0.02%, which is a very small number for a risk, even though the profit is small when compared to the initial capital
- But in calculating the target value, only region 2 shows a profit, where the other regions only show a loss
- The results of the target value in region 2 produce a profit of $3,646,019 with a risk of only 0.097%, this proves that region 2 can be considered for development, seen from the target calculations and predictions which both show absolute profits


## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
