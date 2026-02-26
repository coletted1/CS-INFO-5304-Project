# CS-INFO-5304 Project — World Happiness Report Analysis

**Team:** Tara Munjuluri, Sahithya Swaminathan, Colette D'Costa

## Project Overview

This project uses the World Happiness Report dataset to study country-level well-being and quality of life. We investigate which economic, social, health, and institutional factors are most strongly associated with happiness scores, and how those relationships vary across regions and over time (2011–2024).

## Repository Structure

```
├── Phase1_Dataset_Feasibility.ipynb   # Phase 1 notebook (data collection & cleaning)
├── data/
│   └── final/
│       ├── phase1_analysis_ready.csv          # Full dataset (2011–2024, ~1,969 rows)
│       └── phase1_predictors_complete.csv     # Predictor-complete subset (2019–2024, ~872 rows)
└── README.md
```

## Data Sources

| File | Source | Coverage |
|---|---|---|
| `WHR25_Data_Figure_2.1v3.xlsx` | [World Happiness Report 2025](https://www.worldhappiness.report/data-sharing/) | 2011–2024, 168 countries |
| `DataForFigure2.1WHR2024.xls` | [WHR 2024 Appendix](https://happiness-report.s3.amazonaws.com/2024/DataForFigure2.1WHR2024.xls) | 2021–2023, 143 countries |

## Key Notes on Data

- Predictor columns (`gdp_per_capita`, `social_support`, etc.) are only populated for **2019–2024**. Earlier rows contain the ladder score and rank only.
- The year 2013 is absent from the dataset (no WHR report was published that year).
- The `phase1_predictors_complete.csv` file contains only rows with all six predictors present and is the primary input for regression analysis in Phase 2.

## Research Questions

1. Which country-level factors are most strongly associated with higher happiness scores?
2. Which countries outperform or underperform relative to their economic resources?
3. How have disparities in happiness-related predictors changed over time?