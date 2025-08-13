# Income and Breast Cancer Mortality Rates by NJ Counties (1990–2020)

## Author: Jaquelyn Hester

This project investigates the potential relationship between income and cancer mortality rates across New Jersey counties from 1990 to 2020.

## Introduction

Cancer is a devastating disease that affects many people. This project examines whether income per capita correlates with cancer mortality rates across New Jersey counties.
### Data Sources

Cancer Mortality Rates – Crude mortality rates by county (1990–2020), sourced from the New Jersey State Cancer Registry.

Formula:

    Crude Cancer Mortality Rate = (Deaths from cancer / Population) * 100,000

Income per Capita – County-level income data, sourced from the Bureau of Economic Analysis.

## Data Cleaning and Preparation
Cancer Mortality Data

1. Combined individual CSV files for each year into a single data frame.

2. Selected relevant columns: County, Population at Risk, Deaths, Crude Mortality Rate, Year.

3. Converted Year from character to numeric.

Income Data

1. Extracted county-level per capita income.

2. Pivoted data from wide to long format and then back to wide to align Year and Income columns.

3. Cleaned and arranged data for analysis.

## Exploratory Data Analysis
Cancer Mortality Trends
- Most counties showed relatively steady or declining crude mortality rates from 1990–2020.
- Top 5 counties with the lowest average mortality, displayed using flextables in the HTML output.
- Top 5 counties with the highest average mortality, displayed using flextables in the HTML output.

Income Trends
- Income per capita increased across all counties over time.
- Differences in income levels between counties are visible and persistent.

Animated Scatter Plots

Visualizations explore the relationship between income and mortality rates:

- High Income, Low Mortality Rate: Hunterdon, Morris, and Somerset counties consistently had high income and low mortality rates.
- Low Income, High Mortality Rate: Salem, Atlantic, Cumberland, and Ocean counties had low income and high mortality rates.

Alternative Relationships
- High Income, High Mortality: Bergen and Monmouth (mainly in the 1990s).
- Low Income, Low Mortality: Hudson and Passaic.

Animations are created using gganimate and gifski_renderer().
## Conclusions
1. Higher income generally correlates with lower cancer mortality rates.
2. Lower income generally correlates with higher cancer mortality rates.
3. Exceptions exist, possibly due to demographics, access to care, or other factors.
