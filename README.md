# Weather Conditions and Online Mood In Türkiye DSA210-Project
# Project Overview
This project investigates how weather conditions influence collective mood and online behavior in Türkiye. Using meteorological data from OpenWeather and Google Trends search frequencies for emotion- and activity-related keywords, the study aims to identify correlations between environmental factors and public emotional patterns. Through data preprocessing, visualization, and statistical analysis, it seeks to reveal how variations in temperature, sunlight, and precipitation correspond with changes in well-being and digital engagement across Türkiye.
# Objectives
**Understand Environmental Influences on Mood:**

Examine how key weather variables — including temperature, sunlight hours, and precipitation — correspond with shifts in online mood indicators across Türkiye.

**Analyze Online Behavioral Patterns:**

Investigate changes in public online activity and emotional tone using Google Trends data on Turkish keywords related to depression, stress, happiness, and leisure activities.

**Quantify Weather–Mood Relationships:**

Use statistical and correlation analysis to identify significant relationships between environmental conditions and online behavior, determining which weather factors most strongly influence mood fluctuations.

**Apply Data Science Techniques:**

Use Python and visualization tools to clean, analyze, and interpret real-world datasets, demonstrating how data science can uncover behavioral insights about collective mood and environmental impact.
# Motivation
Mood and behavior are closely tied to people's surroundings, yet these effects are often studied from psychological rather than data-driven perspectives. In a country like Türkiye, where climate patterns vary sharply between regions and seasons, weather can significantly influence emotional well-being and daily routines and with the outcomes of the study, rippling emotions may be interpreted more beneficially.
# Datasets

## Weather Data

**Source:** Meteostat or OpenWeather API

**Data Format:** CSV/Excel (daily observations aggregated to weekly averages)

**Date Range:** January 2022 – December 2024

**Variables Collected:**

Average temperature (°C)

Sunlight duration (hours per day) or cloud coverage (%)

Total precipitation (mm)

**Usage:** Meteorological data will be aggregated weekly to match Google Trends frequency.
These variables represent independent factors influencing collective mood and online activity.
If multiple cities (e.g., Istanbul, Ankara, Izmir) are used, their averages will approximate national climate trends.

## Internet Activity Data

**Source:** Google Trends

**Data Format:** CSV (weekly search interest values on a scale from 0 to 100)

**Region:** Türkiye

**Date Range:** January 2022 – December 2024

**Keywords are grouped into indices:**

NegativeIndex = mean(depresyon, kaygı, stres, üzgün)

PositiveIndex = mean(mutlu, motive, huzurlu, keyifli)

ActivityIndex = mean(YouTube, Netflix, evde kal, sıkıldım)

The dataset will serve as the dependent variable, reflecting public emotional and behavioral trends.

Data will be merged with weather variables by week for comparative and regression analysis.
