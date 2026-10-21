# SmogWatch: Daily PM2.5 Patterns in 15 Pakistani Cities

**Report generated:** 2026-10-21

## 1. Project overview

SmogWatch analyses daily PM2.5 estimates for 15 Pakistani cities from
January 2019 through May 2026. It examines differences between cities,
monthly and yearly patterns, and associations between PM2.5 and weather.

## 2. Data source and methodology

The dataset description identifies the PM2.5 source as the Copernicus
Atmosphere Monitoring Service (CAMS), operated by ECMWF, accessed and
processed through Google Earth Engine. The dataset reports PM2.5 in
micrograms per cubic metre (µg/m³).

These values are model-derived estimates averaged over an approximately
20 km radius around each city's coordinates. They are not direct
ground-monitor measurements and should not be treated as regulatory-grade
observations.

Daily weather variables were retrieved separately from the Open-Meteo
historical archive API. Weather variables include mean temperature,
precipitation, and mean wind speed.

## 3. Data quality

- Records analysed: 40,605
- Cities: 15
- Period: 2019-01-01 to 2026-05-31
- Missing PM2.5 values: 0
- Missing temperature values: 0
- Missing wind speed values: 0
- Missing precipitation values: 0

The current merged dataset has no missing values in the four analysis
variables. This describes completeness, not necessarily measurement accuracy.

## 4. City comparison

### Average PM2.5 by city

             mean  median     max  count
city                                    
Lahore      78.96   63.08  294.61   2707
Faisalabad  72.27   57.46  264.47   2707
Gujranwala  69.22   57.75  299.46   2707
Sialkot     65.94   55.91  230.52   2707
Multan      64.02   52.67  240.60   2707
Sargodha    59.72   50.75  228.73   2707
Bahawalpur  52.49   43.78  232.41   2707
Larkana     46.81   42.31  180.75   2707
Rawalpindi  45.49   41.57  171.14   2707
Islamabad   44.40   40.68  169.10   2707
Sukkur      43.14   36.32  192.10   2707
Karachi     37.01   27.18  208.24   2707
Peshawar    33.00   31.27  106.35   2707
Hyderabad   32.64   25.94  162.18   2707
Quetta      19.66   17.55   86.14   2707

**Finding:** Lahore has the highest average PM2.5 in this dataset,
while Quetta has the lowest. These are comparisons of model-derived
estimates, not official ground-monitor rankings.

## 5. Monthly patterns

- January: 81.17 µg/m³
- February: 60.60 µg/m³
- March: 45.42 µg/m³
- April: 37.80 µg/m³
- May: 40.59 µg/m³
- June: 40.20 µg/m³
- July: 37.18 µg/m³
- August: 33.21 µg/m³
- September: 37.85 µg/m³
- October: 49.79 µg/m³
- November: 65.45 µg/m³
- December: 81.17 µg/m³

**Finding:** January has the highest monthly average,
while August has the lowest in this dataset.
Seasonal patterns may vary by city and year.

## 6. Yearly patterns

- 2019: 72.15 µg/m³
- 2020: 45.97 µg/m³
- 2021: 54.62 µg/m³
- 2022: 45.43 µg/m³
- 2023: 42.72 µg/m³
- 2024: 44.74 µg/m³
- 2025: 50.74 µg/m³
- 2026: 52.25 µg/m³ (partial year: through May)

**Important:** 2026 covers only January through May, so its average should
not be compared directly with full-year averages as if coverage were equal.

## 7. Weather correlation analysis

- PM2.5 vs Temperature: r = -0.368
- PM2.5 vs Wind speed: r = -0.299
- PM2.5 vs Precipitation: r = -0.107

Negative correlations indicate that higher weather-variable values tend
to coincide with lower PM2.5 values in the combined data. Correlation does
not establish causation. These overall correlations may also reflect
seasonality, differences between cities, and other unmeasured factors.

## 8. Recommendations

1. Use validated ground-monitor data when making public-health or
   regulatory decisions.
2. Investigate unusually high estimated PM2.5 values rather than deleting
   them automatically.
3. Examine city-specific and seasonal patterns before drawing conclusions.
4. Treat weather correlations as associations, not proof of cause and effect.
5. Compare with WHO guidelines only with clear disclosure that the dataset
   contains model estimates and that averaging periods are compatible.
6. Document data sources, missing-value handling, and dataset limitations.

## 9. Limitations

- PM2.5 values are model-derived estimates, not direct station readings.
- City values represent an approximate spatial buffer, not every location
  within a city.
- Weather data come from a separate source and may have different spatial
  characteristics from the PM2.5 estimates.
- Overall correlations can hide differences between cities and seasons.
- This analysis alone cannot establish health effects or regulatory compliance.

## 10. Conclusion

SmogWatch provides a reproducible exploratory analysis of daily PM2.5
estimates across 15 Pakistani cities. It identifies city-level differences,
monthly and yearly patterns, and associations with weather. The findings
are useful for exploration and hypothesis generation, while conclusions
about actual exposure and regulatory compliance require validated monitoring
data and careful interpretation.
