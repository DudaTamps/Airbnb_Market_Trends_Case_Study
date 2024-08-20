# Airbnb Market Trends

## Overview

Welcome to New York City, one of the most-visited cities in the world. With high demand for temporary lodging for travelers, the city offers a wide variety of Airbnb listings that cater to both short-term stays and extended periods. This project aims to analyze the Airbnb market in New York by using 2019 data from different sources and formats, including .csv, .tsv, and .xlsx files.

This project was inspired by and based on a case study conducted on the [DataCamp](https://www.datacamp.com/) platform.

## Quick links:
[Data Source](https://www.datacamp.com/) 
[Notebook](https://github.com/DudaTamps/airbnb_market_trends/blob/main/notebook%20(1).ipynb)
[Tableau viz](https://public.tableau.com/app/profile/eduarda.tampelini/viz/AirbnbMarketTrends/Painel1)

## Project Structure

The data used in this project is distributed across three files:

- *data/airbnb_price.csv*: Contains information on Airbnb listing prices and locations.
  - *listing_id*: Unique identifier for the listing.
  - *price*: Nightly listing price in USD.
  - *nbhood_full*: Name of the borough and neighborhood where the listing is located.

- *data/airbnb_room_type.xlsx*: Contains descriptions of the listings and room types.
  - *listing_id*: Unique identifier for the listing.
  - *description*: Description of the listing.
  - *room_type*: Room type (shared room, private room, entire home/apartment).

- *data/airbnb_last_review.tsv*: Contains information on host names and last review dates.
  - *listing_id*: Unique identifier for the listing.
  - *host_name*: Name of the host.
  - *last_review*: Date when the listing was last reviewed.

## What Was Done

In this project, using *Python Pandas*, we performed the following steps:

### 1. Data Import and Unification
- *Data Import*: Imported the different .csv, .xlsx, and .tsv files.
- *Data Unification*: Used the primary key listing_id to merge the data, consolidating all information into a single dataset.

### 2. Data Cleaning and Preparation
- *Standardizing Capitalizations*: Adjusted the room_type column, which had inconsistent capitalization, to ensure uniformity.
- *Data Type Conversion*: Removed the word "dollar" from the price column and converted the variable type to float, allowing proper monetary value manipulation.

### 3. Exploratory Analysis and Insights
- *Room Type Summation*: Summed the number of available private rooms.
- *Key Insights*:
  - *First Review*: Identified the date of the first review.
  - *Last Review*: Identified the date of the last review.
  - *Average Price*: Calculated the average price of stays.
  - *Number of Private Rooms*: Quantified the number of available private rooms.

### 4. Visualizations in Tableau
link: https://public.tableau.com/app/profile/eduarda.tampelini/viz/AirbnbMarketTrends/Painel1
In addition to the Python analysis, some visualizations were created in *Tableau* to illustrate specific insights:
- *Average Prices by Neighborhood*: An overview of the average stay prices across different neighborhoods in New York.
- *Average Prices by Room Type*: A comparison of average prices among room types (shared room, private room, entire home/apartment).
- *Average Airbnb Prices in Manhattan*: Focused on the average stay prices in different parts of Manhattan.
![image](https://github.com/user-attachments/assets/84eff697-a6e1-4042-8288-b6572739de1d)


These visualizations help to better understand price trends and the distribution of available room types in New York.

