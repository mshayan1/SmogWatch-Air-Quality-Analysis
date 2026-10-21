# SmogWatch: PM2.5 Analysis Across Pakistani Cities

## Overview
This project explores 15 cities using 40,605 daily PM2.5 records
from 2019-01-01 through 2026-05-31.

## Data quality and provenance
- Rows analyzed: 40,605
- Cities: 15
- Missing PM2.5 values after cleaning: 0
- Duplicate city-date pairs after deduplication: 0
- PM2.5 source: **Not yet independently verified**
- PM2.5 units: **Not yet verified**
- Weather source: Open-Meteo Historical Weather API, if download succeeded.
- Weather records downloaded: 29,788

## Findings
1. Lahore has the highest average PM2.5 in this dataset (78.96, units unverified).
2. Quetta has the lowest average PM2.5 in this dataset (19.66, units unverified).
3. January has the highest monthly average across available records (81.17, units unverified).
4. August has the lowest monthly average across available records (33.21, units unverified).
5. These are descriptive patterns in the supplied dataset; source, units, and measurement methods must be verified before interpreting them as real-world pollution findings.

## Recommendations
1. Verify the PM2.5 dataset publisher, collection method, and units.
2. Investigate unusual high values against the source before removing or changing them.
3. Use additional validated monitoring data to investigate city and seasonal patterns.
4. Treat weather correlations as associations, not proof that weather caused PM2.5 changes.
5. Compare with WHO guidelines only after confirming the pollutant units and matching averaging periods.
6. Document data limitations and avoid presenting estimates as official measurements.

## Methods
Daily weather values were requested by city coordinates and merged with PM2.5 by city and date.
Charts and summary tables are generated from the available matched data.

## Limitations
The source and units of the supplied PM2.5 values have not yet been verified.
Weather data is an estimate for city coordinates and does not prove pollution causation.
Correlation does not establish causation. WHO comparisons are not included because units and
averaging compatibility have not been verified. The final year may be incomplete.
Review source provenance, API completeness, and missing weather rows before publication.
