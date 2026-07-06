# Washington State EV Population Data Analysis

Exploratory data analysis of Washington State electric vehicle registration data in a Jupyter notebook.

## Overview

This repository contains a Jupyter notebook that analyzes electric vehicle population data for Washington State. The notebook downloads the dataset from Kaggle via `kagglehub`, loads it with pandas, and produces interactive Plotly visualizations alongside printed statistical summaries. The analysis covers EV growth over time, manufacturer and model distribution, geographic patterns by county and city, vehicle type trends (BEV vs PHEV), market share evolution, and CAFV eligibility breakdowns. The notebook is exported in two formats: a standard `.ipynb` file (`EV_Population_Data`) and a percent-format script (`EV Population Data Analysis`).

## Tech Stack

- Python
- Jupyter Notebook
- pandas
- NumPy
- matplotlib
- seaborn
- plotly (express and graph_objects)
- kagglehub

## Features

- Downloads data from Kaggle dataset `sanjanaonteru/electric-vehicle-population-data`
- Data preprocessing: numeric conversion of `Model Year`, column name stripping
- Dataset overview: total EV count, year range, unique manufacturers and models
- Interactive growth timeline (annual registrations and cumulative population)
- Manufacturer/model hierarchy sunburst chart (top 10 makes, top 5 models each)
- County treemap for geographic distribution (top 20 counties)
- BEV vs PHEV adoption bar chart by model year (2010+)
- Top 15 cities horizontal bar chart
- Top 5 manufacturer market share area chart (2015+)
- CAFV eligibility donut chart
- Printed statistical summary (vehicle types, top manufacturers/models, recent growth 2020–2026)

## Getting Started

1. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn plotly kagglehub jupyter
```

2. Open and run the notebook:

```bash
jupyter notebook "EV_Population_Data"
```

Alternatively, run cells from the percent-format script `EV Population Data Analysis` in a compatible environment.

3. Run the first cell to download the Kaggle dataset. Subsequent cells load `Electric_Vehicle_Population_Data.csv` and generate visualizations.

Note: Kaggle authentication may be required for `kagglehub.dataset_download()`.

## Project Structure

```
ev_population_data_analysis/
├── EV_Population_Data              # Jupyter notebook (.ipynb)
└── EV Population Data Analysis     # Percent-format notebook script
```

## Dataset / Results

- **Source:** [Kaggle — Electric Vehicle Population Data](https://www.kaggle.com/datasets/sanjanaonteru/electric-vehicle-population-data) (`sanjanaonteru/electric-vehicle-population-data`)
- **Primary file:** `Electric_Vehicle_Population_Data.csv`
- **Scope:** Washington State EV registrations; model years span roughly 1999–2026
- **Output:** Interactive Plotly charts displayed inline and a printed summary of distributions and growth metrics (no model training or predictions are implemented)
