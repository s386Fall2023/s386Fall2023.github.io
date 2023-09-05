---
title: "NOT FINISHED - Week 5: Pandas"
layout: single
author_profile: false
classes: wide
excerpt: pandas practice
---

## Part 1:  Flights Data 

The data for part can be found in the [homework-data repository](https://github.com/esnt/Data).  

In the **Flights** directory there are several datasets containing information about fights
departing from the New York City area during the year 2013.  Origin airports included are LaGuardia Airport (LGA), John F. Kennedy International Airport (JFK) and Newark Liberty International Airport (EWR).  See the file *data-info.md* or *data-info.pdf* for information about the variables
in each of the datasets.   

Answer the questions below. 

#### Questions using only the *flights.csv* dataset:

1.  How many entries are in the dataset?
2.  Which variable has the most missing values?  How many missing values are there for this variable?
3.  What is the average `air_time` for the flights in the dataset?  
4.  How many unique `dest`s (destinations) are in the dataset?  
5.  What are the five most common destinations for the flights in the dataset?
6.  What is the maximum `distance` flown in the dataset? 
7.  How many flights in the dataset flew the maximum `distance`?  
8.  Create a variable that indicates whether or not a flight was cancelled based on whether or not the `air_time` variable is missing. 
      * What month has the highest proportion of cancelled flights?  What is that proportion?
      * What origin has the lowest proportion of cancelled flights? What is that proportion?
9.  Which date has the largest average arrival delay (`arr_delay`)?  What is that average?
10.  Each plane in the dataset has a unique `tailnum`.  
      * What is the `tailnum` of the most common plane in the dataset? 
      * How many times is it in the dataset? 
      * What is the average `distance` that the plane traveled?  
      * What is the most common route (origin to destination) traveled for this plane? 

#### Questions that require information from one or more other datasets in the **Flights** folder:

11. How many planes have a missing date of manufacture?
12. What is the oldest plane that flew from New York City airports in 2013?
13. What is the correlation coefficient between the number of seats on a plane and the average distance it traveled?
14. How many *days* had precipitation in the New York area in 2013? (That is, how many days had precipitation at at least one of the airports in the dataset at least one of the hours.)
15. Using only days with precipitation greater than zero, what is the correlation between precipitation and average minutes of departure delay?

## Part 2: Practice with missing values, hierarchical indexing, and dropping variables

Use the "happiness_small.csv" data that is included in this repository to answer these questions.  Use python to find the answers.

16. Write a line of code that counts the number of missing values in every column. (Assume that the DataFrame is called `df`.)
17. Process the data using the following steps (using "NA" specific functions)
     * Drop all rows that have missing values in *all* of the "life_expect", "freedom" and "generosity" columns
     * Fill in the remaining missing values in the "generosity" column using the mean of that column  
     * Fill in the remaining missing values in the "freedom" column using forward fill
     * Fill in the remaining missing values in the "life_expect" column with the value 70
     * Fill in the missing values in the "logGDP" country specific median for logGDP
     * After following these steps, report the mean of each column of "logGDP" - "generosity"
18. Using the dataset you made in (17), do the following and write the line of code required for each part on the answer file assuming the DataFrame is called `df`. 
     * (a) Set the "country" column as the index of the dataframe
     * (b) Set the "year" column as the second-level index 
     * (c) Use the hierarchical index to select all the rows cooresponding to 2018
     * (d) Group the dataframe by the first-level index and calculate the mean of each group
     * (e) Group the dataframe by both the first and second-level indexes and calculate the mean of each group.
19. Reset the index back to the original indexing (write the code)
20. Show two ways to drop the "ladder" column