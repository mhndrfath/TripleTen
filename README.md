# Goal
Identifying the top taxi companies, neighborhoods with the most drop-offs, and conducting hypothesis testing

# Data Description
Neighborhood table: data regarding areas in the city of Chicago
- `name`: region name
- `neighborhood_id`: area code
- `Cabs` table: taxi related data
- `cab_id`: vehicle code
- `vehicle_id`: vehicle technical ID
- `company_name`: name of the company that owns the vehicle

Trips table: travel related data
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
- `description`: a short description of the weather conditions, such as "light rain" or "scattered clouds".

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
- `duration_seconds` : trip duration in seconds

# Libraries
pandas, matplotlib, scipy, numpy, nltk

# Content
- Introduction
- Data Overview
- Explorative Data Analysis
- Hypothesis Testing
