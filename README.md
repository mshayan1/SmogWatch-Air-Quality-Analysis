# SmogWatch: Air Quality Analysis in Pakistan

## Project Overview
SmogWatch explores daily PM2.5 estimates across 15 Pakistani cities
from January 2019 to May 2026, alongside historical weather data.

## Objectives
- Compare pollution estimates across cities.
- Explore monthly and yearly trends.
- Analyze relationships between PM2.5 and weather variables.
- Visualize findings using charts and an interactive visualization.

## Tools
Python, Pandas, Matplotlib, Seaborn, Plotly, Google Colab.

## Data Sources
Air quality: CAMS/ECMWF estimates processed through Google Earth Engine.
Weather: Open-Meteo historical archive.

The processed dataset contains 40,605 records across 15 cities.
Fifteen source rows with missing PM2.5 values were excluded.

## Key Findings
- Lahore mean PM2.5 estimate: approximately 78.96 µg/m³.
- Quetta mean PM2.5 estimate: approximately 19.66 µg/m³.
- PM2.5 vs temperature Pearson correlation: -0.368.
- PM2.5 vs wind speed Pearson correlation: -0.299.
- PM2.5 vs precipitation Pearson correlation: -0.107.

Correlations do not establish causation.

## Important Limitations
PM2.5 values are model-derived estimates, not direct ground-monitor
measurements. WHO comparisons are indicative and should not be used
alone to establish regulatory compliance or individual health risk.
The 2026 data covers January through May only.

## Outputs
City summaries, seasonal and yearly trends, heatmaps, distribution
charts, weather correlations, WHO guideline context, an interactive
chart, and a final Markdown report.

## Future Improvements
Add ground-monitor data, build a Power BI dashboard, and explore
pollution forecasting.

## Author
Muhammad Shayan
