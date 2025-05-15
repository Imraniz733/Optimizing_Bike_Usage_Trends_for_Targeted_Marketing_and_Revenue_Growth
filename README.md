# Optimizing Bike Usage Trends for Targeted Marketing and Revenue Growth

## Overview
This project analyzes the cyclistic bike-share dataset to determine how can cyclistic maximize the number of annual memberships  by converting casual riders to members and uncovering usage patterns among casual and member users. The goal is to understand user behavior to improve marketing strategies and operational efficiency.

**For a detailed explanation including code refer to the full interactive report: 👉[ To View Interactive Report](Cyclistic-Bikeshare-Analysis.pdf)**

## Project Description
Cyclistic is a bike-sharing program in Chicago that features more than 5,800 bicycles and 600 docking stations. This analysis focuses on understanding how casual riders and annual members use Cyclistic bikes differently. The insights derived from this project will help Cyclistic's marketing team design targeted campaigns to convert casual riders into annual members.

## Data
The data for this analysis was sourced from the Cyclistic bike-share data provided by Motivate International Inc.,[URL](https://divvy-tripdata.s3.amazonaws.com/index.html). It includes information on ride_id, rideable_type, start and end time, start and end station id or name, start and end lng or lat, member_casual. Data preprocessing included removing duplicate entries, handling missing values, and converting time data to a suitable format.

## Analysis and Methodology

The analysis involved the following steps:

1. **Data Cleaning:** Removed eight column names, start_station_name, start_station_id, end_station_name, end_station_id, start_lat, start_lng, end_lat and end_lng. These columns have missing values in some CSV files and don’t relate to our analysis.
In some CSV files, I have found different length id and keep them as it is because they will not affect our data and those entries are few.
The data is cleaned by applying functions like is.na, duplicated entries, trim, checking the class of columns by lapply, and summary function to check all columns have the same rows min max of date column to check data consistency.

2. **Exploratory Data Analysis:** Summary statistics, data visualization, and Descriptive Analysis
3. **Comparative Analysis:** Comparing ride behaviors between casual users and members.
4. **Visualization:** Creating plots and charts to represent data insights using R and Tableau.

The analysis was conducted using the spreadsheet, R, and the visualizations were created in Tableau.

## Results and Findings

- **Usage Patterns:** Casual riders tend to use the bikes more on weekends, while members have a more consistent usage pattern throughout the week. Additionally, casual riders prefer electric bikes, while members show a preference for classic bikes.
- **Ride Duration:** Casual riders typically have longer ride durations than members.

- **Analysis Summary:**
1. **Classic Bikes:** Classic bikes are used by both casual and member users. However, member users show a higher and more consistent usage pattern across the week compared to casual users.
**Member users:**
   The highest number of rides is observed on day 3 (Wednesday), with 268,250.
   Usage remains relatively stable, with minor fluctuations, ending the week with 227,226 rides on day 7 (Sunday).
**Casual users:**
   Usage starts strong on day 1 (Monday) with 158,107 rides but experiences a significant drop in the middle of the week, reaching a low of 95,820 rides on day 3 (Wednesday).
   There's a recovery towards the end of the week, with 196,665 rides on day 7 (Sunday).
**Interpretation:** Members prefer classic bikes for commuting, showing a steady pattern throughout the week, while casual users, likely influenced by external factors like weather or events, show more variability.

2. **Docked Bikes** Docked bikes are almost exclusively used by casual users, with very limited or no usage by members.
**Member users:**
   No significant usage was observed.
**Casual users:**
   The number of rides starts at 35,295 on day 1 (Monday) and decreases steadily, hitting a low of 17,155 on day 4 (Thursday).
   Usage then increases towards the weekend, peaking at 40,505 rides on day 7 (Sunday).
**Interpretation:** Docked bikes are primarily favored by casual users, especially during the weekend, possibly for leisure or recreational activities. The lack of member usage suggests that this bike type may not meet the needs or preferences of regular commuters.

3. **Electric Bikes** Electric bikes are popular among both casual and member users, with member users again showing higher engagement throughout the week.
**Member users:**
   Electric bike usage starts strong with 225,937 rides on day 2 (Tuesday).
   The number of rides peaks at 264,806 on day 5 (Friday) and then slightly decreases to 215,949 on day 7 (Sunday).
**Casual users:**
   Usage starts at 186,132 rides on day 1 (Monday) but shows a dip in the middle of the week, reaching 149,865 rides on day 3 (Wednesday).
   There’s a steady increase towards the end of the week, with 235,062 rides on day 7 (Sunday).
**Interpretation:** Electric bikes are well-utilized by both user groups, with members consistently favoring them for their likely convenience and speed. Casual users also show a strong preference, particularly towards the weekend, indicating a possible combination of commuting and leisure use.

## Conclusion
The analysis of bike usage across different types and user groups reveals distinct patterns:
- Classic Bikes are favored by members for consistent use throughout the week, with casual users showing more fluctuation.
- Docked Bikes are predominantly used by casual users, particularly during the weekend, while members show little to no interest.
- Electric Bikes are popular among both casual and member users, with members showing a higher and more consistent usage.

These insights can inform operational decisions, such as bike availability, marketing strategies, and membership promotions, ensuring that the needs of both casual and member users are met effectively.

## Recommendations
- Cyclistic should focus on converting casual riders to annual members by promoting weekday benefits.
- Increase availability of classic bikes during peak casual rider times.
- Launch targeted marketing campaigns for casual riders during weekends.

