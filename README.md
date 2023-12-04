# Goal
Selecting the plan with the highest potential revenue for different target markets and conducting hypothesis testing

# Data Description
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

# Libraries
*pandas, matplotlib, scipy, numpy, nltk*

# Content
- Introduction
- Data Overview
- Data Pre-Processing
- Statistical Data Analysis
- Hypothesis Testing
- General Conclusion
