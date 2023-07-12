# Recall Data Analysis

This repository contains code for analyzing and visualizing recall data for NHTSA (National Highway Traffic Safety Administration) campaigns using Python. 


## Libraries used

[![Library](https://img.shields.io/badge/Library-Pandas%2C%20NumPy%2C%20Matplotlib%2C%20Seaborn%2C%20NLTK-orange.svg)](https://pypi.org/)

The code leverages popular libraries such as Pandas, NumPy, Matplotlib, Seaborn, and NLTK to load, profile, clean, analyze, and visualize recall data from a CSV file.

## Code Overview

The code performs the following tasks:

- Imports the necessary libraries: Pandas, NumPy, Matplotlib, Seaborn, and NLTK.
- Loads the recall data from the "Recalls_Data.csv" file into a Pandas DataFrame.
- Conducts data profiling and cleaning operations, including checking data types and null values, changing column names, and converting data types.
- Generates summary statistics and displays the head and tail of the DataFrame.
- The dataset has data from the year 1966 until 2023. There are only three recall incidents in 2023
- Filters the dataset to only focus on recalls in 2022.
- Removes outliers using the interquartile range
- Performs analysis and visualization tasks on the number of recalls for the year 2022, such as 
    1. Plot the number of recalls by type - Most recalls happenned in vehicular category
    2. Find the top 10 Manufacturers by number of recalls - Daimler Trucks North America had the largest number of recalls in 2022, followed by Volkswagen and Forest River.
- Performs analysis and visualization tasks on the number of people affected for the year 2022, such as 
    1. Plot the number of people affected by recall type - Most number of people are affected by vehicular recalls
        On Further analysis, on an average, tire calls affect more number of people than vehicular recalls.
        However, there is more variation in the number of people affected by tire recalls as compared to vehicular recalls. 
    2. Find the top 10 Manufacturers by number of people affected - Volkswagen affected the largest number of people in 2022, followed by Chrysler, Ford, Navistar and Mercedes-Benz.
- Conducts text analysis on the consequence summary, including tokenization, removal of stop words and punctuation, lemmatization, and frequency analysis. The top 20 most common words are plotted in a bar chart.

Data Source - https://data.world/makeovermonday/2023w4 | U.S. Department of Transportation 

[def]: https://github.com/your-username/repo-name/blob/main/LICENSE