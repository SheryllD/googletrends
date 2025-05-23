# PyTrends Time Series Analysis

This repository contains a Jupyter Notebook that uses the `pytrends` API to analyse the popularity of selected keywords over time. The project focuses on identifying trends, seasonality, and residual patterns within Google search interest data.

## Overview

This project demonstrates how to:

- Connect to Google Trends via the `pytrends` API
- Retrieve historical interest data for specific search terms
- Visualise search trends for multiple keywords
- Perform time series decomposition to uncover underlying components

This notebook explores search activity in the United States over the past five years using examples such as `bitcoin`, `ethereum`, and `dogecoin`, `blockchain`, `nft`.

## Installation

To run this notebook, install the following Python packages:

```bash
pip install pytrends pandas matplotlib seaborn statsmodels

```

## Recuirements 
- Written for Python 3.3+
- Requires Requests, lxml, Pandas


## Usage
1. Open the pytrends.ipynb notebook.
2. Define the keywords of interest.
3. Retrieve and inspect the trend data.
4. Visualise the trends over time.
5. Apply seasonal decomposition to one or more keyword time series.

## API 

<pre> 
from pytrends.request import TrendReq # Example usage: pytrends = TrendReq(hl='en-US', tz=360) </pre>

NOTE: You can also use proxies if you're blocked due to Google's rate limits.

<pre> 
from pytrends.request import TrendReq pytrends = TrendReq( hl='en-US', tz=360, timeout=(10, 25), proxies=['https://34.203.233.13:80'], retries=2, backoff_factor=0.1, requests_args={'verify': False} )  </pre>

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