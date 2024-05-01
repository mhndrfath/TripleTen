# Vehicle Price Analysis

## Project Description
The task involves conducting an analysis at Crankshaft List, where hundreds of free vehicle ads are posted on the website daily. The objective is to examine datasets spanning the past few years to identify the factors that impact the price of a vehicle.

## Data Description
Dataset is stored in files `vehicle_in_us.csv`

Column Description :
- `price`
- `model_year` - year of manufacture
- `model` - car type
- `condition` - car condition
- `cylinders` - number of cylinder on the engine
- `fuel` — gas, diesel, etc.
- `odometer` — distance traveled by the vehicle when the ad was shown
- `transmission`
- `paint_color`
- `is_4wd` — whether the vehicle has 4 wheel drive (Boolean type)
- `date_posted` — the date the ad aired
- `days_listed` — the number of days the ad ran until it was removed

## Methodology
- Data Overview (Check general information of dataset)
- Data Pre-Processing (Further check, handle missing value and fix data type)
- Explorative Data Analysis (Data quality checking, observe outlier, etc)

## Result
The objectives of this analysis include:
1. Select data that will later be used to make conclusions
2. Look at what parameters influence the sales of a vehicle
3. Analyze what factors most influence the price of a vehicle

After analysis, the data answered these objectives with several statements for general conclusions:
1. The initial data used in this analysis is still very dirty, among other things
- missing data that has been handled by creating a new column by filling in the missing values with the median of the column related to the other column references
- outlier data that has been removed by taking certain limits to make it easier for potential buyers
- different data types have been replaced with proper ones
2. In general, there are many parameters that influence the sale of a vehicle, such as price, mileage, age of the vehicle, color of the vehicle, year of manufacture of the vehicle, type of vehicle transmission

3. In particular, there are several factors that greatly influence the sales of a vehicle, such as
- the price definitely has an absolute influence
- the distance traveled by a vehicle can affect the performance of a vehicle's engine
- the year a vehicle was manufactured and the age of the vehicle from its first owner

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
