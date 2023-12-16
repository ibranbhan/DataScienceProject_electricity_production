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
The core problem we want to solve is to predict the total electricity production in GWh for a country. using these variables
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
- Data source:
https://www.kaggle.com/datasets/ccanb23/iea-monthly-electricity-statistics
- Number of rows: 
181915
- Number of Features:
12
- The size of df is 181915 rows x 12 features.
- The data file size is 18.7 MB
  
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

# Model Selection
Random Forest Regressor:

Reasoning:
Handles non-linear relationships well, crucial for predicting electricity generation with complex patterns.
Robust to outliers, providing stability in irregular data points.
Incorporates feature importance rankings, aiding in understanding key predictive features.
Gradient Boosting Regressor:

Reasoning:
Builds an ensemble of weak learners to capture intricate relationships in data.
Effective for non-linear dependencies, suitable for complex energy generation datasets.
High accuracy and mitigates overfitting through sequential model building.
Support Vector Regression (SVR):

Reasoning:
Effective in high-dimensional spaces, aligning with the multidimensional nature of the dataset.
Flexible kernel function choice to handle various data relationships.
Suitable for non-linear dependencies significant in predicting electricity generation

  # Conculsion

In conclusion, the predictive models were evaluated based on their Mean Absolute Error (MAE) performance metrics. The MAE values for each model are as follows:

Random Forest Regressor MAE: 674.87

The Random Forest model demonstrated superior performance with a low MAE, indicating accurate predictions.
Its ability to handle non-linear relationships, robustness to outliers, and feature importance rankings contributed to its success.
Gradient Boosting Regressor MAE: 21652.76

The Gradient Boosting model exhibited a higher MAE compared to Random Forest, suggesting a less accurate predictive performance.
Despite its effectiveness in capturing complex patterns, the model may require further tuning to enhance accuracy.
Support Vector Regression (SVR) MAE: 20788.34

The SVR model displayed a similar MAE to Gradient Boosting, indicating room for improvement.
SVR's effectiveness in capturing complex relationships in high-dimensional spaces suggests potential, but further optimization may be beneficial.
In summary, while the Random Forest Regressor outperformed the other models in terms of MAE, ongoing refinement and optimization of the Gradient Boosting and SVR models may lead to improved predictive accuracy. These insights contribute to the iterative process of model development, guiding future efforts to enhance the effectiveness of electricity generation predictions.
