# Weather Conditions and Online Mood In Istanbul DSA210-Project
# Project Overview
This project investigates how weather conditions influence collective mood and online behavior in Istanbul. Using meteorological data from OpenWeather and Google Trends search frequencies for emotion- and activity-related keywords, the study aims to identify correlations between environmental factors and public emotional patterns. Through data preprocessing, visualization, and statistical analysis, it seeks to reveal how variations in temperature, sunlight, and precipitation correspond with changes in well-being and digital engagement across Istanbul.
# Objectives
**Understand Environmental Influences on Mood:**

Examine how key weather variables — including temperature, sunlight hours, and precipitation — correspond with shifts in online mood indicators across Istanbul.

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

**Region:** Istanbul

**Date Range:** January 2022 – December 2024

**Keywords are grouped into indices:**

NegativeMoodIndex =  mean(depresyon, kaygı, anksiyete, stres, bunalım)

PositiveMoodIndex = mean(mutlu, mutluluk, huzurlu, iyi hissetmek)

NegativeBehaviorIndex = mean(yalnızlık, uykusuzluk, yorgunluk)

PositiveBehaviorIndex = mean(spor salonu, yürüyüş)

The dataset will serve as the dependent variable, reflecting public emotional and behavioral trends.

Data will be merged with weather variables by week for comparative and regression analysis.

# Hypothesis
## H1 — Temperature and Positive Mood
Higher average temperature is associated with higher PositiveMoodIndex since warmth generally increases outdoor activities and social interactions, which promotes positive mood.
## H2 — Rain and Negative Mood
Weeks with measurable rainfall have higher NegativeMoodIndex than dry weeks due to rain and low sunlight being linked to stress, lethargy, and low affect.
## H3 — Temperature Variability and Mood Instability
Weeks with extreme temperature swings correlate with greater variance in mood indices.

# Methodology
## Data Collection

Weather data was collected using the Meteostat API (daily observations).
**Variables include:**
tavg, tmin, tmax, precipitation, snow, wind speed, pressure, sunlight duration.

Google Trends search activity was collected using the Pytrends library.
Keywords were grouped into emotional and behavioral categories (negative mood, positive mood, negative behavior, positive behavior).
## Data Preprocessing

Daily weather data was aggregated into weekly averages to match Google Trends' weekly frequency.

Missing values were inspected using heatmaps and handled through forward/backward filling where appropriate.

Google Trends “isPartial” values were removed.

Weekly weather data and Google Trends data were merged into a single dataset using date alignment.
## Exploratory Data Analysis (EDA)

Summary statistics (mean, median, std)

Histograms and boxplots for all weather variables

Correlation matrix visualized via heatmaps

Missing value analysis

Weekly trends plotted to observe seasonal patterns
## Statistical Analysis

Several statistical models and tests were applied:

Pearson correlation between weather variables and mood/behavior indices

Independent t-tests (e.g., rainy vs non-rainy weeks)

Chi-square tests for categorical weather conditions (rainy/non-rainy) vs high/low mood groups

One-way ANOVA to examine whether mood indices differ under different temperature groups

These tests evaluate whether observed relationships are statistically significant.

