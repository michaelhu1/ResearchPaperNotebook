# CO2 Emissions & Climate Change Perception Analysis

Research notebook for a published paper in Vanderbilt University's Young Scientists Journal (May 2023).  
**[Read the paper](https://wp0.vanderbilt.edu/youngscientistjournal/article/providing-recommendations-on-combating-climate-change-through-data-driven-analysis)**

## What this is

This project uses machine learning to find what factors actually drive a country's CO2 emissions — 
and whether public awareness of climate change has any measurable effect on national sustainability.

Data was pulled from the Pew Research Center, World Bank, UN, and CIA World Factbook across 37 countries.

## Key findings

- In republics (where citizens have more political influence), public perception of climate change 
  had a meaningful negative correlation with CO2 emissions per capita — suggesting that educating 
  citizens matters
- What looks like a correlation between agriculture and lower emissions is actually a GDP effect: 
  wealthier countries tend to have less agricultural activity, not the other way around
- After controlling for GDP, industrial activity was the only sector with a direct positive 
  correlation to CO2 emissions (p = 0.053)

## Models

- **Random Forest Regression** — predicts CO2 emissions per capita from 12 country-level features; 
  23.6% mean error on republic countries (39.5% overall, pulled up by two outliers)
- **OLS Regression** — adjusted R² of 0.832 on republic countries

## Stack

Python · pandas · scikit-learn · statsmodels · seaborn · matplotlib

## Authors

Michael Hu & Mauricio Hernandez (Duke University)  
Conducted through the Lumiere Research Scholar Program
