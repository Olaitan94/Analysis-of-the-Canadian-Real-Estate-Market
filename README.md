# Analysis-of-the-Canadian-Real-Estate-Market
Analysing the trends in the canadian real estatemarket from October 2022 to January 2023

## Project Motivation 
The canadian real estate market has been a hot topic of news since 2021 due to the hike in prices of properties. The mortage rates were increased to crash the prices. But has this been effective or are the prices still on the rise? 

For this project, I analyzed the real estate market in the major cities (population of over 200,000) in the Prairies & West Coast Regions of Canada to answer the following questions: 

- **How effective has the increase in mortgage rate been in crashing the market?**
- **What cities have the highest demand?**
- **Where would you advise someone with limited funds to buy a house?**
- **How well can we predict the price of a house?**

## Data
To answer these questions, I obtained the following data:
   - Houses sold in Major cities in the Prairie & West Coast regions from **Sept 25, 2022 to January 30, 2023**. (*Source: scraped from honestdoor.ca*) 
      - Major cities include: Winnipeg, Calgary, Edmonton, Vancouver, Burnaby, Surrey, Regina, Saskatoon
   - Population of major cities in 2021 (*Source: Wikipedia*)
   - 5 - year fixed mortgage rates in Canada from September to January (*Source: ycharts.com*) 

## Summary of Analysis & Results

1. **How effective has the increase in mortgage rate been in crashing the market?**
    - To get an idea of the effect of the increase in mortgage rates on the market, I performed a month-to-month comparison of the average prices of houses sold and total no of houses sold (demand) in each city. 
   - From the Analysis, Both the average prices and the total no of houses sold in eah city have reduced signifcantly from October, 2022 to January, 2023. Thus,there is evidence that the increase in mortgage rates have reduced the avergae prices & demand for houses. 

2. **What city has the highest demand?**
   - After analysisng the total number of houses sold in each city during the period, I discovered that Calgary has had the highest no of sales in each month and then concluded that Calgary has the highest demand.
   - I performed a comparison of Demand vs Population for each city and discovered that there is a direct relationship between these two. The population in Calgary is significantly higher than other cities and this is likely the cause of the higher demand in Calgary.

3. **Where would you advise someone with limited funds to buy a house?**
   - My approach to answering this question was to focus on the reason for buying the house: Residential or Investment purposes.
   - For residential purposes, I considered the average prices in each of the cities, the years the houses were built & the number of bedrooms and concluded that Regina is the best place to buy a house because you can get newer bigger houses for less.
   - For investment purposes, I considered the budget of the investor, the demand & avegrage prices in each city & concluded that Investors with less than 500k USD should get a hous in Edmonton while Investos with over 500k CAD should get a house in Calgary.

4. **How well can we predict the price of a house?**
   - The Last part of this project involved training a model with this data to predict price of a house.
   -  To train this model,I prepared the data by
      - removing columns that were not useful( Columns with ID & account number) and columns that had just one value.
      - Imputing missing values in some columns and removed columns that had too many missing values.
      - Checking for and removing outliers
   - Implemented a linear regression model (with & without regularization), evaluated the performance of the model on the test set and amde recommendations


## File Descriptions
1. Analyzing_the_Real_Estate_Market_in_Canada.ipynb: This notebook contains the complete code, analysis and visualizations that address the questions.
2. House_Price_Prediction.ipynb: This notebook contains the complete code for cleaning the data, training and evaluating the price prediction model
3. Plots: This folder contains png files of all the plots created during the analysis
4. canada_house_prices.csv: This file contains the data on houses sold in the cities being considered from sept 25 to jan 30,2023
5. mortgage_rates.txt: This file contains data on the mortage rates in canada from september 2022 to january 2023
6. population.txt: This file contains data on the population in the cities in 2021

## Installation
Python version: 3.9
Tools: Jupyter Notebook
Libraries:
   - Pandas
   - Numpy
   - Sklearn
   - Matplotlib
   - Seaborn
