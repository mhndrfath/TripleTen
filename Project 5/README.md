# Video Game Analysis

## project Description
At the online store "Ice," where video games from around the world are sold, an analyst is tasked with identifying patterns to determine the success of a game using data from 2016. This data includes user and expert game reviews, genre, platform (e.g., Xbox or PlayStation), and historical game sales information sourced from open databases.

The objective is to pinpoint factors that contribute to a game's success or lack thereof. By analyzing this data, the analyst aims to identify games with the highest potential and strategize advertising campaigns for 2017.

The dataset contains abbreviations, such as ESRB, which stands for Entertainment Software Rating Board—an independent regulatory organization that evaluates game content and assigns age ratings like Teen or Mature.

## Data Description
Dataset is stored in files `games.csv`

Column Description
- `Name` (name)
- `Platforms`
- `Year_of_Release` (year of release)
- `Genres`
- `NA_sales` (sales in North America in million USD)
- `EU_sales` (sales in Europe in million USD)
- `JP_sales` (sales in Japan in million USD)
- `Other_sales` (sales in other countries in million USD)
- `Critic_Score` (review score from critics, maximum 100)
- `User_Score` (review score from users, maximum 10)
- `Ratings` (ESRB)

## Methodology
- Data Overview
- Data Pre-Processing
  - Rename Columns
  - Handle Missing Values
  - Change type of data
- Data Analysis
  - Review game and sales
  - Data Collection time period
  - Reviews influnce on sales
  - General Distribution of games
- User Profile
  - 5 Top platform
  - 5 Top genre
  - ESRB Rating
- Testing Hypothesis

## Result
After analyzing the overall data and testing the hypothesis, we arrive at the final conclusion. Where there are several changes that have been made such as:
- In the 'user score' and 'critic score' columns which have null data, they have been filled with median which refers to the genre column, where these two columns will be used to see the correlation with total sales, which in fact these two columns do not have a very significant influence on sale
- From 1980 - 2016, the biggest sales occurred in 2008, where in that year game consoles such as PS2 and others appeared.
- Even though the PS2 holds the record for the most sales since 1980, the PS2 does not really influence the analysis because the data period used in further analysis is only data from the last 5 years
- High sales only occur when a console is released, thus creating outliers that are far from the average range

General conclusions that can be drawn from data analysis for game campaigns in 2017 include:
- The 'Action' genre is the genre with the most sales throughout 2012 - 2016, which could possibly further increase the quality and quantity of this genre for the following year
- PS4 is the platform with the most sales in the last 5 years, so game producers can focus on this platform
- Ratings 'E' and 'M' are 2 ratings that indicate consumer interest in all regions
- Game producers can ask for suggestions from professional users to improve the quality of games that will be produced in the following year

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
