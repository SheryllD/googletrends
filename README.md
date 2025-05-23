# PyTrends Time Series Analysis

This repository contains a Jupyter Notebook that uses the `pytrends` API to analyse the popularity of selected keywords over time. The project focuses on identifying trends, seasonality, and residual patterns within Google search interest data.

## Overview

This project demonstrates how to:

- Connect to Google Trends via the `pytrends` API
- Retrieve historical interest data for specific search terms
- Visualise search trends for multiple keywords
- Perform time series decomposition to uncover underlying components

The notebook uses examples such as `chatgpt`, `ai`, and `deepseek`, focusing on search activity within Germany over the past five years.


## Requirements

To run this notebook, install the following Python packages:

```bash
pip install pytrends pandas matplotlib seaborn statsmodels

```

## Usage
1. Open the pytrends.ipynb notebook.
2. Define the keywords of interest.
3. Retrieve and inspect the trend data.
4. Visualise the trends over time.
5. Apply seasonal decomposition to one or more keyword time series.

## Methodology
The analysis follows these main steps:
- Connect to Google Trends with regional and time filters
- Retrieve interest data using pytrends.build_payload
- Display and inspect the resulting time series
- Plot trends to compare keyword interest
- Use statsmodels to decompose a selected time series into trend, seasonality, and residuals

This structure allows for both exploratory analysis and preparation for future predictive modelling.

## Future Improvements
- Apply decomposition to additional keywords
- Integrate forecasting techniques such as ARIMA or Prophet
- Combine trend data with external datasets for richer insights

## Author
Sheryll Dumapal.

Building responsible, data-driven tools with clarity and purpose.