# CS215_FinalProject_Arvin
# Air Pollution in Ulaanbaatar, Mongolia

## Project Overview

This project studies air pollution in Ulaanbaatar, Mongolia using daily air quality data and daily weather data from 2016 to 2019. The goal of the project is to understand how pollution changes over time, how it differs across monitoring stations, and how weather conditions are associated with daily pollution levels.

## Main Research Questions

1. How do major air pollutants in Ulaanbaatar vary across seasons and years?
2. Which monitoring stations show the worst pollution levels, and do stations group into different pollution profiles?
3. How are daily weather conditions associated with air pollution levels?

## Data Sources

This project uses the following main data sources:

- **OpenAQ API** for air quality data in Ulaanbaatar
- **Daily weather data** for Ulaanbaatar covering temperature, precipitation, wind speed, and snowfall
- **Approximate station coordinate data** used for the station map visualization

## Main Techniques Used

The project uses several data analysis techniques, including:

- data wrangling and cleaning
- grouping and aggregation
- creation of cleaned and derived datasets
- k-means clustering for station pollution profiles
- geographic visualization using station coordinates
- correlation analysis between pollutants and weather variables
- multiple linear regression for PM2.5 and weather relationships

## Main Findings

Some of the main findings from the project are:

- Most major pollutants are much worse in winter than in summer, especially **SO2**, **PM2.5**, and **CO**
- **O3** behaves differently from the other pollutants and tends to be higher in warmer conditions
- Pollution is not evenly distributed across monitoring stations, and some parts of the city consistently show higher particulate pollution
- The clustering analysis suggests that stations can be grouped into different multi-pollutant profiles
- Temperature is the strongest weather-related factor in the dataset, with colder days associated with much worse **PM2.5**, **SO2**, and **CO**
- A simple regression model showed that temperature and wind speed were both meaningfully associated with PM2.5 levels

## Folder descriptions
- notebooks/ contains the main project notebooks
  - CS215_FinalProject_DATA.ipynb contains data collection, cleaning, and dataset preparation
  - CS215_FinalProject_ARVIN.ipynb contains the final analysis, visualizations, and interpretation
- data/ contains all the datasets used for this project
- figures/ contains exported figures from the final notebook

## Limitations

This project has a few important limitations:

- not every monitoring station measured every pollutant
- some station-level clustering required filtering and simple imputation
- the station map uses approximate coordinates rather than exact official station boundaries
- the weather analysis shows associations between variables, but it does not prove causation

## Credits

This project used course materials, DataCamp modules, and outside tools for debugging and workflow support. ChatGPT was used at some points to help think through coding issues.
