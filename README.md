# Zomato Data Analysis
## Project Overview:
This project performs an in-depth exploratory data analysis (EDA) of a Zomato restaurant dataset to uncover critical business insights and understand the factors influencing 
restaurant ratings and popularity. The goal is to explore key variables—such as restaurant type, service availability (online ordering, table booking), 
and cost—to identify trends that can inform business strategy and provide a comprehensive view of the local restaurant landscape.

## Dataset:
File Used: Zomato data .csv
The dataset represents a collection of restaurant records with attributes vital for market analysis:
- name,
- online_order,
- book_table,
- rate,
- votes,
- approx_cost,
- listed_in(type)
It provides a robust foundation for studying service trends, cost distributions, and customer engagement metrics (ratings and votes).

## Data Cleaning and Preprocessing:
- Loaded the dataset into a DataFrame.
- Checked for and handled missing values, particularly in the critical *rate* column, using an appropriate imputation or removal strategy.
- Rate Conversion: The *rate* column was converted from a string format (e.g., '4.1/5') to a clean numerical float type (e.g., 4.1) by splitting and casting, making it suitable for mathematical operations and statistical analysis.
- Removed duplicates and ensured consistency in categorical columns (e.g., standardizing text/case).

## Feature Engineering:
Derived new columns for qualitative interpretation:
- Rate Categories: Grouped the clean numerical *rate* column into bins (e.g., Excellent, Good, Average, Low) for easier descriptive analysis.
- Cost Categories: Categorized *approx_cost* into descriptive buckets (e.g., Budget, Mid-Range, Premium) to analyze pricing strategies.

## Exploratory Data Analysis (EDA):
The EDA section uses the cleaned data to deeply examine trends and distributions across various dimensions:
a. General Distribution:
- Frequency of restaurants by *listed_in(type)* to identify the most common restaurant categories (Dining is dominant).
- Distribution of *approx_cost* to find the most common price points.

b. Ratings and Votes:
- Distribution of the numerical rate column using histograms.
- Analysis of the top-rated restaurants.
- Distribution of votes to understand customer engagement across different restaurant types.

c. Service-Level Insights:
- Comparison of average ratings for restaurants that offer *online_order* vs. those that do not.
- Comparison of average votes for restaurants that offer *book_table* vs. those that do not.
- Analysis of which restaurant types are most likely to offer online ordering and table booking.

d. Correlation Analysis:
- Relationship between votes and rate to see if higher engagement correlates with better ratings.
- Relationship between *approx_cost*(for two people) and rate.

## Data Visualization:
- Bar Charts/Countplots: Summarizing the frequency of restaurant types and service availability (online/booking).
- Histograms/KDE plots: Showing the distribution of the numerical rate and approx_cost columns.
- Boxplots: Comparing the spread of ratings and votes across key categorical variables (e.g., comparing rate distribution between 'Yes' and 'No' for online ordering).
- Heatmaps/Correlation Plots: Analyzing the relationship between numerical features.

## Insights & Findings:
From the analysis, key insights include:
- The Dining type of restaurant is the most prevalent category in the dataset, accounting for the majority of entries and total votes.
- The majority of restaurant ratings cluster in the 3.5 to 4.0 range, indicating a competitive and generally well-rated market segment.
- Restaurants that offer online ordering tend to have a slightly higher average rating than those that do not.
- The most common and accessible price point for two people is generally around 300.
- There is a noticeable difference in customer engagement: restaurant types like 'Dining' receive higher vote counts than more niche types.

## Tools and Libraries:
- Python: Core language
- Libraries: Pandas, NumPy, Matplotlib, Seaborn
- Environment: Jupyter Notebook
- Techniques: Data Cleaning, Data Pre-processing, Exploratory Data Analysis (EDA), Data Visualization

## Deliverables:
- Cleaned and preprocessed dataset ready for further modeling.
- Clear visual insights summarizing key trends in the restaurant industry.

## Summary:
This project demonstrates an end-to-end data analysis workflow, transforming raw Zomato data into actionable insights through meticulous preprocessing, 
feature engineering, and visual storytelling. It effectively highlights the factors driving restaurant popularity and ratings, showcasing your ability 
to handle real-world data and communicate findings effectively.
