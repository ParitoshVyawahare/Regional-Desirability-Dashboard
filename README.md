# Howard County Desirability Dashboard  

## Overview  
This project focuses on creating an interactive dashboard that evaluates the desirability of various regions in Howard County, Maryland. By analyzing multiple socioeconomic variables, the dashboard provides an overall score for each ZIP code and highlights the most desirable regions. The dashboard was developed using Tableau for visualization and Python for data preprocessing.  

## Data Sources  
The data for this project was collected from reliable sources, including:  
- **U.S. Census Bureau**: Employment status, total population, poverty status, and mean income by ZIP code. ([Source](https://data.census.gov/table))  
- **Zillow**: Housing prices by ZIP code. ([Source](https://www.zillow.com/research/data/))  

## Variables Used  
The analysis is based on the following variables:  
1. **Total Population**  
2. **Employment Status**  
3. **Mean Income**  
4. **Housing Prices**  
5. **Poverty Status**  

## Methodology  
### 1. Data Preprocessing  
- Used Python for data cleaning and standardization.  
- Applied **Z-score standardization** to normalize the data.  
- Performed **Min-Max scaling** to ensure values fell between 0 and 1.  

### 2. Weight Allotment  
Each variable was assigned a weight based on its relative importance in determining desirability:  
- Total Population: 15%  
- Mean Income: 30%  
- Housing Prices: 10%  
- Employment Status: 35%  
- Poverty Status: 10%  

### 3. Overall Score Calculation  
The overall score for each ZIP code was calculated using the following steps:  
- Multiply the normalized value of each variable by its assigned weight.  
- Sum the weighted scores for all variables.  
- Divide the total score by the number of variables (5).  

## Insights from the Dashboard  
The dashboard provides the following insights for Howard County:  
- Cities like **Columbia** and **Ellicott City** achieved the highest overall scores due to low poverty rates and high employment levels, making them the most desirable locations within the county.  
- The interactive map visualizes overall scores for each ZIP code, offering an easy comparison of desirability across regions.  

## Dashboard Features  
- **Map Visualization**: Displays overall scores by ZIP code.  
- **Heatmaps**: Highlight variability in scores across regions.  
- **Bar Charts**: Compare mean income, employment, and other variables for each city.  

## Tools and Technologies  
- **Tableau**: Created an interactive dashboard for visualizing insights.  
- **Python**: Preprocessed data and calculated scores.  
- **Excel**: Handled initial data formatting and organization.  

## How to Access the Dashboard  
The dashboard is hosted on Tableau Public and can be accessed via the link below:  
[Howard County Desirability Dashboard](https://public.tableau.com/views/HowardCountyDesirabilityDashboard/HowardDasboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)  

## Conclusion  
Howard County’s desirability was successfully analyzed based on multiple socioeconomic variables. The dashboard provides actionable insights and a comprehensive visualization of desirability scores across ZIP codes.
