---
layout: default
title: California Wildfire Forecast Prediction
description: Forecasting wildfire activity across California using historical fire, weather, and geographic data.
---

# California Wildfire Forecast Prediction

## Overview

This project investigates whether historical weather and geographic information can be used to understand and forecast wildfire activity across California.

The project combines wildfire records, weather observations, and California county boundaries to create a county-level weekly dataset for analysis and future forecasting.

## Research Question

Can historical weather conditions and geographic information help predict wildfire activity across California?

## Data

The project combines three primary datasets:

### California Fire Records

The CalFire dataset contains approximately 18,000 recorded fires across California from 1950–2025.

Important variables include:

- Fire name
- Fire start date
- Fire cause
- Acres burned
- Geographic location

### Weather Data

The weather dataset contains approximately 467,000 daily observations from California weather stations.

Variables include:

- Average temperature
- Relative humidity
- Average wind speed
- Maximum wind speed
- Precipitation

### California County Boundaries

County boundary shapefiles are used to associate wildfire locations with California counties.

## Data Preparation

The datasets were cleaned and combined into a weekly county-level modeling dataset.

Major steps included:

1. Cleaning and converting date variables
2. Assigning weather stations to counties
3. Cleaning wildfire records
4. Performing a spatial join between fires and county boundaries
5. Aggregating weather observations by county and week
6. Aggregating wildfire activity by county and week
7. Combining the weather and wildfire datasets

The resulting dataset contains weekly weather conditions and wildfire activity for California counties.

## Exploratory Data Analysis

The analysis investigates several patterns in wildfire activity.

### Fire Activity Over Time

Weekly wildfire counts were analyzed to identify changes in wildfire activity over time.

### Geographic Distribution

Wildfire activity was mapped across California counties to identify areas with higher concentrations of fires.

### Seasonality

Monthly and weekly patterns were analyzed to investigate wildfire seasonality.

### Weather Relationships

Temperature, humidity, wind speed, and precipitation were compared with wildfire activity.

## Statistical Analysis

Several statistical methods were used to investigate relationships between weather conditions and wildfire activity.

### Correlation Analysis

Weather variables were compared with weekly wildfire counts.

Temperature showed a positive relationship with wildfire activity, while humidity and precipitation showed negative relationships.

### Welch's t-test

Hot and cold weeks were compared using a Welch two-sample t-test to investigate whether wildfire activity differed between temperature groups.

### Poisson Regression

A Poisson regression model was used to estimate the relationship between weekly wildfire counts and weather variables.

The model includes:

- Average temperature
- Average humidity
- Average wind speed
- Total precipitation

## Current Status

This project is currently in development.

Completed:

- Data collection
- Data cleaning
- Geographic processing
- County-level spatial joins
- Weekly aggregation
- Exploratory data analysis
- Statistical analysis
- Initial Poisson regression

Next steps:

- Feature engineering
- Machine learning models
- Time-series forecasting
- Model evaluation
- Feature importance analysis
- Forecast visualization

## Technologies

- Python
- Pandas
- GeoPandas
- NumPy
- Matplotlib
- Plotly
- SciPy
- Statsmodels
- Statistical Modeling
- Geospatial Analysis
- Machine Learning
- Git & GitHub
