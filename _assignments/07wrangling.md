---
title: "Week 7: Data Wrangling"
layout: single
author_profile: false
classes: wide
excerpt: Practice wrangling skills
---

## Part 1

Finish the Regex Lab we started in class on March 7:

1. Load the "employee.csv" data into a Pandas DataFrame (this data can now also be found in the Data Repo)
2. Use regular expressions to extract the first and last names from the "name" column and create two new variable called "first_name" and "last_name"
3. Use regular expressions to extract the area code from the phone number column and create a new variable called "area_code"
4. Use regular expressions to extract the year from the "birthdate" column and create a new variable called "birthyear"
5. Use regular expression to extract the city and state from the "mailing_address" and create two new variables called "city" and "state"
6. Create a column that is the length of the job title, excluding punctuation and special characters
7. Create a columns that shows the height in inches
8. Create a column that contains the domain of the email addresses (e.g. "yahoo.com")
9. Create a variable that computes the age at the time of starting (use pd.to_datetime)
10. Keep only the new variables that you created in parts (2)-(9).  
11. Save the new data frame, called "employee_clean.csv" and include it in this repository.

## Part 2
In the **MessyData** directory, the "mexico_weather.csv" dataset contains information from a weather station in mexico from 1955 - 2011.  The weather variables included are tmax (maximum daily temperature), tmin (minimum daily temperature), and prcp (daily precipitation).  

For the "mexico_weather.csv" data, clean and tidy the data so that: 
- There are seven columns:  year, month, day, date, tmax, tmin, prcp
    - The "date" variable should be a "datetime" variable with the Year-month-day
- Values 999 and 9999 are missing values and should be replaced with NaN (np.nan)
- There are no rows corresponding to nonsensical dates (e.g., April 31)
- Rows in which tmax, tmin, and prcp are all missing are dropped (note that dropping these rows will also take care of invalid dates)
- The non-missing values for tmax, tmin, and prcp are to be divided by 10 (for example, the value 310 should be 31.0)
- Answer the following questions about the data:    
    a. How many rows are there in the tidy dataset?  
    b. What is the overall mean of tmax (maximum daily temperature)?    
    c. What is the mean across years of tmin (minimum daily temperature) on August 1.    
    d. What date (month/day/year) has the largest prcp (daily precipitation)?  
    e. What is the value of the largest prcp?   
    f. Which month has the largest average difference between tmin and tmax?
- Save your cleaned data as "mexico_weather_clean.csv" and include it in this repository.

## Part 3
In the **MessyData** directory, the "TB2022.csv" contains data downloaded from the [WHO](https://www.who.int/teams/global-tuberculosis-programme/data) about the number of tuberculosis cases by country.  This data was recently downloaded but only contains information for the years 2012-2020.  

For the "TB2022.csv" data, tidy and clean the dataset so that:
- There are six columns: country, region (g_whoregion), year, sex, age, cases
- The age categories are 0-14, 15-19, 20-24, 25-34, 35-44, 45-54, 55-64, 65+
    - Ideally the values of your age variable correspond to the categories listed above, however, it's okay if you leave the values as 014, 1519, 2024, 2534, 3544, 4554, 5564, 65
- Sort the data by country then year then sex then age.  Fill missing cases using both the forward- and backward-fill methods
- Answer the following questions about the data:      
        a. Using the forward-fill method, what is the mean number of cases for females aged 55-64?    
        b. Using the backward-fill method, what is the mean number of cases for females aged 55-64?      
        c. What sex/age combination has the largest difference between the ffill and bfill methods?   
        d. What sex/age combination has the smallest difference between the ffill and bfill methods? 
- Save your cleaned data as "TB2022_clean.csv" and include it in this repository.
