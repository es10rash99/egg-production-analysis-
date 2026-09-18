# Environmental Effect on Egg Production — Exploratory Data Analysis

## Overview
This project analyzes how environmental conditions inside poultry housing (temperature, humidity, ammonia, light intensity, noise, feeding amount) affect egg production rate. It combines hands-on poultry/hatchery domain knowledge with a Python-based data analysis workflow.

## Motivation
As a Poultry Hatchery Lab Engineer, I regularly monitored environmental conditions (temperature, humidity, ventilation) as part of incubation management. This project applies statistical and data analysis techniques (Python, Pandas, scikit-learn) to the same type of data, to quantify which factors actually drive production performance rather than relying on observation alone.

## Dataset
- 481 daily records from a poultry farm
- Features: number of chickens, feeding amount, ammonia level, temperature, humidity, light intensity, noise, total egg production
- Source: Kaggle — "Environmental Effect on Egg Production"

## Methods
1. Data cleaning and exploration (no missing values found)
2. Created a fairer performance metric: `Production_Rate = Total_egg_production / Amount_of_chicken`
3. Correlation analysis between environmental factors and production rate
4. Linear Regression model to quantify each factor's individual effect
5. Temperature binning to identify the optimal temperature range

## Key Findings
- **Temperature** is the strongest environmental driver of egg production rate among the factors tested.
- **Ammonia** and **noise** show a mild negative relationship with production rate, consistent with known stress effects on poultry.
- The optimal temperature range in this dataset is approximately **30–31°C**, where average production rate peaks.
- Environmental factors alone (excluding flock size) explain a moderate portion of the variance — flock size itself remains the dominant factor, which is an expected and informative result.

## Tools
Python, Pandas, Matplotlib, Seaborn, scikit-learn

## Files
- `Egg_Production_Analysis.ipynb` — full analysis notebook with code, charts, and explanations
- `Egg_Production.csv` — dataset used

## Author
Esraa Ahmed Ali Eliw — Poultry Hatchery Lab Engineer transitioning into agricultural data analysis.
[LinkedIn](https://linkedin.com/in/esreliw99)
