# Taxi Company Analysis (Effect of Weather on Travel Frequency)

## Project Description
At Zuber, a new ride-sharing company launching in Chicago, the task is to find patterns in the available information. The objective is to understand passenger preferences and the impact of external factors on travel.

Using a database, data from competitors will be analyzed, and hypotheses regarding the effect of weather on travel frequency will be tested.

## Data Description
Dataset are stored in files:
- `project_sql_result_01.csv`
- `project_sql_result_04.csv`
- `project_sql_result_07.csv`

Column Description:
- `neighborhood_id`: area code
- `Cabs` table: taxi related data
- `cab_id`: vehicle code
- `vehicle_id`: vehicle technical ID
- `company_name`: name of the company that owns the vehicle
  
Trips table: travel related data\n",
- `trip_id`: trip code
- `cab_id`: operating vehicle code
- `start_ts`: date and time the trip started (time rounded in hours)
- `end_ts`: date and time the trip ends (time rounded in hours)
- `duration_seconds`: trip duration in seconds
- `distance_miles`: trip distance in miles
- `pickup_location_id`: pickup area code
- `dropoff_location_id`: delivery area code
  
weather_records table: weather related data
- `record_id`: weather recording code
- `ts`: date and time when weather recording was carried out (time rounded in hours)
- `temperature`: the temperature when weather recording was carried out
- `description`: a short description of the weather conditions, such as \"light rain\" or \"scattered clouds\".

From the file above, the following file results are obtained:
  
(project_sql_result_01.csv.) This file contains the following data:
- `company_name`: taxi company name
- `trips_amount`: number of trips for each taxi company on 15-16 November 2017.
  
(project_sql_result_04.csv.) This file contains the following data:
- `dropoff_location_name`: name of the area in Chicago where the trip ends
- `average_trips`: average number of trips ending in each region in November 2017.
  
(project_sql_result_07.csv) — result of the last query.
This file contains travel data from the Loop to O'Hare International Airport. This file contains the following data:
- `start_ts` : pick-up date and time
- `weather_conditions` : weather conditions when the trip starts
- `duration_seconds` : trip duration in seconds"

## Methodology
- Data Overview
- Exploratory Data Analysis
  - Identify 10 regions as drop-off
  - Handling outlier
- Testing Hypothesis

## Result
- Information and intellectual information about web developers is needed for an analyst
- Skills in managing data in SQL are the key to this analysis
- A task elaboration system that can be developed in this project to minimize errors
- Parsing data from websites is very necessary for a data analyst
- Selection and merging of several files into 1 data file is very useful for analysis results
- There are no errors in the data types used in the analysis
- There are no null values which makes it easier for an analyst to process the data
- Outliers that must be considered when testing a hypothesis

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
