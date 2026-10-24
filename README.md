# California Incarceration & Mental Health Access Analysis

## Overview
Does greater access to mental health facilities relate to lower jail incarceration rates across California counties? This project tests the idea that jails have become de facto mental health institutions by comparing facility counts and incarceration rates across California counties from 2020–2024.

## Data
Six public datasets, filtered to California counties, averaged across available years (2020-2024), and merged by county into one dataset:

| Dataset | Source | Used for |
|---|---|---|
| Jail population | [Vera Institute](https://github.com/vera-institute/incarceration-trends/blob/main/People-in-Jail-and-Prison-in-2024-Data.xlsx) | Incarceration rate per county |
| Mental health facilities | [CA Health and Human Services](https://data.chhs.ca.gov/dataset/licensed-mental-health-rehabilitation-centers-mhrc-and-psychiatric-health-facilities-phf/resource/ef9f4daf-892c-45f6-b46a-3037c5a93b23) | Number of facilities per county |
| Median household income | [U.S. Census (ACS)](https://data.census.gov/table/ACSST5Y2020.S1901?q=income&moe=false) | Median income per county |
| Unemployment | [U.S. Census (ACS)](https://data.census.gov/table/ACSDP1Y2023.DP03?g=040XX00US06,06$0500000) | Unemployment rate per county |
| County population | [U.S. Census](https://www.census.gov/data/tables/time-series/demo/popest/2020s-counties-total.html) | Calculating incarceration rates |
| County codes | [CA Health and Human Services](https://data.chhs.ca.gov/dataset/licensed-mental-health-rehabilitation-centers-mhrc-and-psychiatric-health-facilities-phf/resource/ff6478dd-200c-4c44-a545-d32eac14e9fb) | Matching counties across datasets |

## Methods
* Cleaned and merged datasets
* EDA and visualization: explored variable relationships and regional patterns across CA counties with plots such as a correlation heatmap and choropleth maps
* Compared simple and multiple OLS regression models by comparing the adjusted R^2 of each
* **Tools:** pandas, numpy, matplotlib, seaborn, geopandas, statsmodels

## Key Findings

## Files
- `data/` - data folder
  - `ca_county_code_list.csv`: CA county code data
  - `ca_employment_data`: CA employment data
  - `jail_data`: jail incarceration data
  - `income_data`: income data
  - `mental_health_center.csv`: mental health facilities data
  - `population_data`: population data
- `jails_mental_health.ipnyb`: full analysis and write-up Jupyter notebook
- `jails_mental_health_proposal.ipnyb`: original project proposal Jupyter notebook

## Team
Group project by Roxana Chen, Jiayi Xue, Daphne Chen, Andrew Nguyen
