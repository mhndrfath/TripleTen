# Phone Plan Analysis

## Project Description
The task at Megaline involves conducting an initial analysis of the prepaid plans Surf and Ultimate based on a sample of 500 clients. The provided dataset includes information on client demographics, plan subscriptions, and usage metrics like the number of calls and messages sent in 2018.

The objective is to analyze client behavior to determine which prepaid plan generates higher revenue. This analysis will inform decisions regarding advertising budget allocation, aiding in optimizing resource utilization effectively.

## Data Description
Dataset are stored in files
- `megaline_calls.csv`
- `megaline_internet.csv`
- `megaline_messages.csv`
- `megaline_plans.csv`
- `megaline_users.csv`

Users table (user data):
- `user_id` — User ID
- `first_name` — user's first name
- `last_name` — user's last name
- `age` — user's age (years)
- `reg_date` — subscription start date (dd, mm, yy)
- `churn_date` — the date the user stopped using the service (if the value is missing or does not exist, it means the service plan was in use when this data was generated)
- `city` — the city where the user lives
- `plan` — phone plan name

Calls table (call data):
- `id` — Unique web session ID
- `call_date` — call date
- `duration` — call duration (in minutes)
- `user_id` — ID of the user making the call

Messages table (SMS data):
- `id` — Unique SMS ID
- `message_date` — date the SMS was sent
- `user_id` — ID of the user who sent the SMS

Internet tables (web session data):
- `id` — Unique web session ID
- `mb_used` — volume of data consumed during the session (in megabytes)
- `session_date` — web session date
- `user_id` — User ID

Plans table (phone package data):
- `plan_name` — phone plan name
- `usd_monthly_fee` — monthly fee in US dollars
- `minutes_included` — monthly calling minutes allocation
- `messages_included` — monthly SMS allocation
- `mb_per_month_included` — monthly data volume allocation (in megabytes)
- `usd_per_minute` — price per minute if the package allocation limit has been exceeded (for example, if the package has an allocation of 100 minutes, then usage starting from the 101st minute will be charged)
- `usd_per_message` — price per SMS if the package allocation limit has been exceeded
- `usd_per_gb` — price per extra gigabyte of data if the package allocation limit is exceeded (1 GB = 1024 megabytes)

## Methodology
- Data Overview
- Data Pre-Processing
  - Grouping specific columns
  - Dataset merger
- Statistical Data Analysis
  - Surf package
  - Ultimate Package
- Testing Hypothesis

## Result
After analyzing data on cellular data usage among consumers with different package types, it can be concluded that:
    
- The package that gets more revenue is the surf package, seen from the usage of consumers who choose this package more and there are also many consumers whose usage exceeds the package limit obtained
- The New York and New Jersey (NY-NJ) region has a difference in revenue from other regions, seen from the large number (more than other regions) with a significant difference of 14% from other regions

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
