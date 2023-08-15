---
title: "Week 5: Webscraping"
layout: single
author_profile: false
classes: wide
excerpt: Webscraping & APIs
---
## \#1
Using `requests`, `BeautifulSoup`, and `pandas`, create a DataFrame of the
[140 Essential Action Movies](https://editorial.rottentomatoes.com/guide/140-essential-action-movies-to-watch-now/)
as selected by Rotten Tomatoes. 

Your DataFrame should have 140 rows and 4 or 5 columns:

| Title | Year | Score | Rank | (Category) |
| --------|--------|--------|--------|--------|

where 
- "Title" is the movie title, 
- "Year" is the year the movie came out, 
- "Score" is the tomato meter score (NOT the adjusted score), 
- "Rank" is the assigned ranking from 1 to 140.
- "Category" is the rating category used by Rotten Tomatoes and should be "Certified Fresh", "Fresh", or "Rotten" 

"Title" and "Category" should be type "object". "Year","Score", and "Rank" should be type "int".

*Hints*
- The information for each movie is inside a `div` tag with `"class"` = `"col-sm-18 col-full-xs countdown-item-content"`
- "Title", "Year", and "Score" are all inside a heading tag (within the `div` mentioned in the previous bullet)
- "Rank" is found inside a `div` tag (within the `div` mentioned in the first bullet) 
- Suppose that `df` is a pandas DataFrame with variable called "col1" that is of type "object" .  The code 
`df['col1'] = df['col1'].astype(int)` will cast `col1` into an integer.


(a) Report the mean "year" and the mean "score" (rounded to 3 decimal places) on the `hw-03-answers.txt` file.

(b) What is the correlation coefficient between "score" and "rank"

(b) What is the mean "Rank" of each "category".

---

## \#2

Using `pd.read_html` and the following Wikipedia pages:

* [List of United States tornadoes from January to March 2022](https://en.wikipedia.org/wiki/List_of_United_States_tornadoes_from_January_to_March_2022)
* [List of United States tornadoes in April 2022](https://en.wikipedia.org/wiki/List_of_United_States_tornadoes_in_April_2022)
* [List of United States tornadoes from May to June 2022](https://en.wikipedia.org/wiki/List_of_United_States_tornadoes_from_May_to_June_2022)
* [List of United States tornadoes from July to October 2022](https://en.wikipedia.org/wiki/List_of_United_States_tornadoes_from_July_to_October_2022)
* [List of United States tornadoes from November to December 2022](https://en.wikipedia.org/wiki/List_of_United_States_tornadoes_from_November_to_December_2022)

to compile a dataset of US tornadoes in 2022. 


    
 
---
## \#3

For this part, use the [Currency Exchange API](https://exchangeratesapi.io).  You will need to sign up for the FREE plan in order to get an API key.  Using the "timeseries" endpoint, find the exchange rates of the Euro (EUR), the Israeli New Shekel (ILS), the Hong Kong Dollar (HKD), and the British Pound Sterling (GBP) as compared to the US Dollar (USD) from May 1, 2022 through Feb 1, 2023. 

*Hint: All parameters can be entered using a dictionary to the "params" argument in the .get() function.*

Using the result, report the correlation coefficient of the Euro values versus the values for ILS, HKD, and GBP rounded to 3 decimal places.  
