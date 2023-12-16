# Team memebers
* Yahya Mahdali - 220024667
* Abdulrahman Alsubayq - 220016516
* Ibrahim Nabhan - 220034486
* Saleh Alanazi - 221434727

# Introduction 
The landscape of global energy production has been evolving significantly over the past decade, with a marked shift towards renewable sources and an increased focus on sustainable practices. This transition is evident in the comprehensive dataset of 'Monthly Electricity Production in GWh [2010-2022]', sourced from the International Energy Agency (IEA) through their Monthly Electricity Statistics tool.

Spanning over a diverse range of energy products like hydro, wind, solar, geothermal, nuclear, and fossil fuels, the dataset provides a granular view of electricity generation in gigawatt-hours (GWh). The dataset is enriched with detailed classifications, including types of energy products, monthly and yearly breakdowns, and comparative analyses of year-to-date generation figures.

This project is not just a technical endeavor but a crucial step towards a more informed and sustainable future in global energy management. Through the intelligent application of data science techniques, it aspires to contribute to the broader dialogue on energy sustainability and efficiency.

# Problem statment
The core problem we want to solve is to predict the electricity price production in GWh for a country. using these variables
- Name of the country
- The year of the data point
- The month of the data point as a number
- The type of energy product
  
 We will utilize advanced models such as Random Forest Regressor, Gradient Boosting Regressor, and Support Vector Regression (SVR) to uncover patterns, dependencies, and predictive factors in electricity production.

# Objective
The project aims to uncover underlying patterns, dependencies, and predictive factors in electricity production by applying sophisticated data science techniques like Random Forest Regressor, Gradient Boosting Regressor, and Support Vector Regression (SVR).

# Dataset Approach
The primary approach for addressing the analysis of global electricity production trends is to perform a comprehensive examination of monthly electricity production data across various countries from 2010 to 2022. This approach involves aggregating and analyzing data to understand the changes in energy production, with a focus on the transition towards renewable energy sources and the comparison of energy mixes across different nations.

# Dataset Collection
Data Collection:
https://www.kaggle.com/datasets/ccanb23/iea-monthly-electricity-statistics

# Dataset Description
The data includes information about energy production in various countries on a monthly basis from 2010 to 2022. The energy production is measured in gigawatt-hours (GWh) and covers a range of energy products including hydro, wind, solar, geothermal, nuclear, fossil fuels, and others.

Countries:
Argentina, Australia, Austria, Belgium, Brazil, Bulgaria, Canada, Chile, Colombia, Costa Rica, Croatia, Cyprus, Czech Republic, Denmark, Estonia, Finland, France, Germany, Greece, Hungary, IEA Total, Iceland, India, Ireland, Italy, Japan, Korea, Latvia, Lithuania, Luxembourg, Malta, Mexico, Netherlands, New Zealand, North Macedonia, Norway, OECD Americas, OECD Asia Oceania, OECD Europe, OECD Total, People's Republic of China, Poland, Portugal, Republic of Turkiye, Romania, Serbia, Slovak Republic, Slovenia, Spain, Sweden, Switzerland, United Kingdom, United States

Products:
Hydro, Wind, Solar, Geothermal, Other renewables, Nuclear, Total combustible fuels, Coal, Oil, Natural gas, Combustible renewables, Other combustible non-renewables, Not specified, Net electricity production, Total imports, Total exports, Electricity supplied, Used for pumped storage, Distribution losses, Final consumption, Electricity trade, Renewables, Non-renewables, Others, Other renewables aggregated, Low carbon, Fossil fuels

The dataset columns include:
COUNTRY: Name of the country
CODE_TIME: A code that represents the month and year (e.g., JAN2010 for January 2010)
TIME: The month and year in a more human-readable format (e.g., January 2010)
YEAR: The year of the data point
MONTH: The month of the data point as a number (1-12)
MONTH_NAME: The month of the data point as a string (e.g., January)
PRODUCT: The type of energy product (e.g., Hydro, Wind, Solar)
VALUE: The amount of electricity generated in gigawatt-hours (GWh)
DISPLAY_ORDER: The order in which the products should be displayed
yearToDate: The amount of electricity generated for the current year up to the current month in GWh
previousYearToDate: The amount of electricity generated for the previous year up to the current month in GWh
share: The share of the product in the total electricity generation for the country in decimal format

# Dataset Preprocessing:
The preprocessing phase involves cleaning the data for any inconsistencies or missing values, normalizing the data formats, and structuring the dataset for analysis.
This includes:
- Feature Engineering
- Drop columns
- Convert categorical data to numerical data
- Find duplicate values
- Find Null values
- Replace null values with 0

# Data Science Techniques for Analysis:
Time-Series Analysis: 
To examine trends over time, time-series analysis will be employed. This technique is ideal for understanding how electricity production has evolved monthly and annually, highlighting trends and patterns.

# Data Visualization: 
To effectively communicate the findings, various data visualization tools will be used.


  # Conculsion

  In this project, we've undertaken a comprehensive analysis of global electricity production trends from 2010 to 2022 using data from the International Energy Agency (IEA). Our objectives included identifying production patterns, assessing renewable energy growth, and comparing energy mixes across countries. We employed data scraping to collect detailed data, which was then rigorously preprocessed.
    
    During our preliminary analysis, we presented an overview of the dataset and initial findings, such as temporal trends and energy product diversity. We outlined plans for further in-depth analysis, including country-wise assessments, energy product distribution exploration, and seasonal pattern identification.
    
    Visualizations, such as time series plots and bar charts, will support our analysis. This project goes beyond technical analysis, offering insights for policymakers, resource management, sustainability, and economic considerations.
    
    In summary, this project aims to contribute to informed and sustainable global energy management. It leverages advanced data science techniques to uncover underlying electricity production patterns, with significant implications for decision-makers and the broader energy sustainability discourse.
