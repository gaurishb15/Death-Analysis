# Death Rate Analysis

## Project Overview

This project involves analyzing global death rate data from various causes, incorporating additional economic indicators such as the Human Development Index (HDI) and Gross Domestic Product (GDP). The analysis explores gender-wise and country-wise mortality trends, highlighting socio-economic factors influencing these trends.

## Objective

The objective is to provide insights that can help improve health policies by understanding mortality patterns across different demographics and socio-economic conditions. By studying gender-specific death rates and the correlation between HDI and GDP with mortality data, this project aids in identifying key factors that may affect public health policies.

## Data Sources

1. *Death Rates*: Data was sourced using the WHO Global Health Observatory (GHO) API, filtered for gender-wise death rates across multiple causes in 151 countries.
2. *HDI Data*: Scraped from CountryEconomy.com for 172 countries (year 2004).
3. *GDP Data*: Acquired as a CSV from the World Bank (year 2004).

## Code Explanation

The code in this repository processes and visualizes death rate data. Below is an outline of the major steps in the code:

1. *Data Extraction and Cleaning*:
   - The WHO GHO API data is filtered by keywords (e.g., "Death") to obtain mortality-related datasets.
   - JSON files are converted to R data frames and filtered to ensure consistency across datasets (e.g., gender-based segregation and country intersections).
   
2. *Data Integration*:
   - Merged the death rate data with HDI and GDP indicators to allow correlation analysis.
   
3. *Bias Detection*:
   - Implemented checks to assess potential biases due to incomplete data or regional differences in reporting practices.

4. *Visualizations*:
   - Created scatter plots, bar charts, and linear models to illustrate death rate patterns across gender, country development status (developed vs. developing), and specific diseases.

## How to Use the Code

1. *Dependencies*: Ensure that you have the required libraries such as dplyr and ggplot2 installed in your R environment.
   
2. *Running the Analysis*:
   - Load the datasets as outlined in the code. 
   - Execute the data cleaning and transformation steps to ensure consistent data across mortality, HDI, and GDP datasets.
   - Run the visualization scripts to generate charts and graphs that highlight mortality trends and outliers.

3. *Visualizing the Results*:
   - The plots provide a comprehensive view of death rate correlations with socio-economic factors. Modify plot parameters as needed to focus on specific countries or causes.

## Conclusion

This project provides a foundation for analyzing and improving global health policies. By exploring mortality data in conjunction with socio-economic indicators, it sheds light on key trends and outliers, emphasizing the importance of high-quality data in public health decision-making.
