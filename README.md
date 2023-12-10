# forexanalysisalphavantage
forex analysis with real time data from trading view
# Forex Analysis using Alpha Vantage Data

This project involves performing forex analysis using data retrieved from Alpha Vantage's API for the GBP/USD currency pair.

## Overview

The primary objective of this project is to demonstrate the process of retrieving forex daily data using Alpha Vantage's API and performing analysis or building models for GBP/USD currency pair.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/forex-analysis-alpha-vantage.git
    ```

2. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Retrieving Data

To import forex daily data from Alpha Vantage, we use the Python `requests` library to make API requests. The retrieved data is processed and used for analysis or model building.

Example code snippet for data retrieval:

```python
import requests

# Replace the "demo" API key below with your own key from Alpha Vantage
url = 'https://www.alphavantage.co/query?function=FX_DAILY&from_symbol=GBP&to_symbol=USD&apikey=YOUR_API_KEY'
r = requests.get(url)
data = r.json()

print(data)
