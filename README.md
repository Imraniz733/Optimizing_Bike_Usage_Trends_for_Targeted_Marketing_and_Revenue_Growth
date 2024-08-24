# Cyclistic Bike-share Analysis Project
## Overview
This project analyzes the cyclistic bike-share dataset to determine how can cyclistic maximize the number of annual memberships  by converting casual riders to members and uncovering usage patterns among casual and member users. The goal is to understand user behavior to improve marketing strategies and operational efficiency.

## Project Description
Cyclistic is a bike-sharing program in Chicago that features more than 5,800 bicycles and 600 docking stations. This analysis focuses on understanding how casual riders and annual members use Cyclistic bikes differently. The insights derived from this project will help Cyclistic's marketing team design targeted campaigns to convert casual riders into annual members.

## Data
The data for this analysis was sourced from the Cyclistic bike-share data provided by Motivate International Inc,[URL](https://divvy-tripdata.s3.amazonaws.com/index.html). It includes information on ride_id, rideable_type, start and end time, start and end station id or name, start and end lng or lat, member_casual. Data preprocessing steps included removing duplicate entries, handling missing values, and converting time data to a suitable format.

## Analysis and Methodology

The analysis involved the following steps:

1. **Data Cleaning:** Removed eight column names, start_station_name, start_station_id, end_station_name, end_station_id, start_lat, start_lng, end_lat and end_lng. These columns have missing values in some CSV files and don’t relate to our analysis.
In some CSV files, I have found different length id and keep them as it is because they will not affect our data and those entries are few.
The data is cleaned by applying functions like is.na, duplicated entries, trim, check class of columns by lapply, summary function to check all columns have same rows min max of date column to check data consistency.

2. **Exploratory Data Analysis:** Summary statistics, data visualization, and Descriptive Analysis
3. **Comparative Analysis:** Comparing ride behaviors between casual users and members.
4. **Visualization:** Creating plots and charts to represent data insights using R and Tableau.

The analysis was conducted using spreadsheet, R, and the visualizations were created in Tableau.

## Results and Findings

- **Usage Patterns:** Casual riders tend to use the bikes more on weekends, while members have a more consistent usage pattern throughout the week. Additionally, casual riders prefer elctric bikes, while members show a preference for classic bikes.
- **Ride Duration:** Casual riders typically have longer ride durations than members.
- **Analysis summary**:
1. **Classic Bikes**
-**Member users:**
   *The highest number of rides is observed on day 3 (Wednesday), with 268,250 rides.
   *Usage remains relatively stable, with minor fluctuations, ending the week with 227,226 rides on day 7 (Sunday).

These insights suggest that marketing efforts could be tailored to promote weekend offers to casual riders, while members might benefit from incentives for using electric bikes.

