# Horse-Race-Analysis
An end-to-end data pipeline and interactive dashboard analyzing 
betting market efficiency across 5 major U.S. racetracks using 
2023 Equibase past performance data.

## Overview
This project explores how accurately horse racing odds reflect 
true win probability. The dashboard displays actionable 
insights around favorites, longshots, jockeys, and track tendencies.

## Key Findings
- Saratoga had the highest house margin, making it the toughest track for bettors to profit
- Favorites are consistently and accurately priced
- Gulfstream Park showed the most extreme longshot odds, meaning a higher variance in betting opportunities
- A 2026 Kentucky Derby winning jockey appeared as a top jockey-trainer combination in the dataset

## Tech Stack
- **Python** - XML parsing, feature engineering, analysis
- **Pandas** - Data wrangling and aggregation
- **Tableau** - Interactive dashboard
- **Data** - Equibase XML files (2023, 5 major tracks)

## Pipeline
`parse_pp.py -> feature_engineering.py -> analysis.py -> Tableau`

## Files
| File | Description |
|---|---|
| `parse_pp.py` | Parses raw Equibase XML into CSVs |
| `feature_engineering.py` | Engineers market features |
| `analysis.py` | Generates summary tables for Tableau |
| `output/` | CSVs fed into Tableau |

## Dashboard
[See Dashboard](https://public.tableau.com/app/profile/madison.brown7953/viz/HorseRacingAnalysis/Dashboard1?publish=yes)

## Data Source
Equibase past performance XML files  - 5 tracks, 2023 season  
Aqueduct (AQU), Churchill Downs (CD), Del Mar (DMR), Gulfstream Park (GP), Saratoga (SAR)

## Future Improvements
I would like to explore a live dataset to be able to predict winnings in advance.
