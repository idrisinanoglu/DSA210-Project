# Weather Conditions and Online Mood in Istanbul

## Project Overview
This project explores the relationship between weather conditions and collective online mood in Istanbul. By combining meteorological data with Google Trends search frequencies related to emotional states and daily activities, the study aims to investigate how environmental factors may influence public mood and behavior patterns.

The project integrates data preprocessing, exploratory analysis, statistical methods, and machine learning techniques to examine whether weather variables provide meaningful explanatory or predictive power for online mood indicators.

---

## Objectives
- Examine how key weather variables such as temperature and precipitation relate to online mood indicators.
- Analyze public online behavior using aggregated Google Trends search data.
- Explore statistical and machine learning approaches to assess weather–mood relationships.
- Apply data science techniques to a real-world, socially relevant problem.

---

## Motivation
Mood and behavior are closely tied to environmental conditions, yet these effects are often discussed qualitatively rather than analyzed quantitatively. In a country like Türkiye, where seasonal and regional climate variation is pronounced, understanding potential weather–mood relationships may provide insights into collective well-being and behavioral trends.

This project aims to approach the topic from a data-driven perspective by leveraging openly available datasets and analytical tools.

---

## Data Sources
### Weather Data
- **Source:** Meteostat API
- **Content:** Daily weather observations (temperature, precipitation, wind speed, pressure)
- **Processing:** Aggregated to weekly frequency

### Internet Activity Data
- **Source:** Google Trends
- **Content:** Weekly search interest values for emotion- and activity-related Turkish keywords
- **Region:** Istanbul
- **Processing:** Keywords grouped into mood and behavior indices

---

## Method Summary
Daily weather data and weekly Google Trends data are merged at a weekly level. The combined dataset is explored using descriptive statistics and visualizations, followed by statistical hypothesis testing. Machine learning models are then applied as an exploratory extension to assess whether weather variables contain predictive signal for online mood indicators.

---

## Tools and Technologies
- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Meteostat API
- Pytrends

---

## Repository Structure
- `data/` – raw and processed datasets  
- `notebooks/` – data analysis and modeling notebooks  
- `figures/` – generated plots and visualizations  
- `final_report.pdf` – detailed academic report
