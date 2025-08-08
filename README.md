# NBA Award Prediction Project

## Project Overview

This repository contains data mining workflows to predict NBA award winners using statistical analysis. The project focuses on three major awards:

1. Most Valuable Player (MVP)
2. Defensive Player of the Year (DPOY)
3. Sixth Man of the Year (SMOY)

## Directory Structure

```bash
.
├── archive/ # Pristine original datasets (read-only)
│ └── untouched*seasonal_data/ # Raw player stats (1980-2025)
│
├── data/ # All project datasets
│ ├── raw/ # Original unprocessed data
│ │ ├── player_stats/ # Individual season stats (CSVs)
│ │ └── team_stats/ # League standings & win totals
│ │
│ ├── processed/ # Cleaned/transformed data
│ │ ├── player_stats/ # Processed seasonal data
│ │ └── league_standings/ # Compiled team performance data
│ │
│ └── interim/ # Combined datasets for analysis
│ ├── nba_combined*\*.csv # Merged data chunks
│
├── notebooks/ # Jupyter notebooks
│ ├── awards/ # Award-specific analyses
│ │ ├── dpoy/ # Defensive Player models
│ │ ├── mvp/ # MVP prediction workflows
│ │ └── smoy/ # Sixth Man analysis
│ │
│ ├── analysis/ # General statistical tools
│ ├── scraping/ # Data collection scripts
│ └── test/ # Experimental code
│
└── README.md # This document
```

## Key Features

- 40+ years of historical NBA data (1980-2025)
- Automated data processing pipelines
- Award-specific predictive models
- Reproducible Jupyter workflows

## Usage Notes

1. Raw data should never be modified directly
2. Processed datasets are regenerated from raw sources
3. Notebooks assume data lives in ../data/ relative paths

## Methodology

Our models use:

- Regular season performance metrics
- Team success indicators
- Historical voting patterns
- Advanced analytics (PER, WS, etc.)

## Future Work

- Expand to other awards (ROY, MIP)
- Incorporate play-by-play data
- Build interactive visualizations
