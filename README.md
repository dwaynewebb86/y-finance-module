# y-finance-module
The Y Finance Module is a financial module used to fetch financial and market data.

This repository shows the installation of the 'yfinance' module

Link: [https://pypi.org/project/yfinance/](url)

Install Steps
-------------
Y Finance is a non-standard library and requires manual installation

Install yfinance from PYPI using pip:

$ pip install yfinance 

Example
-------

import yfinance as yf

# Define the ticker symbol
ticker_symbol = "AAPL"

# Create a Ticker object
ticker = yf.Ticker(ticker_symbol)

# Fetch historical market data
historical_data = ticker.history(period="1y")  # data for the last year
print("Historical Data:")
print(historical_data)

# Fetch basic financials
financials = ticker.financials
print("\nFinancials:")
print(financials)

# Fetch stock actions like dividends and splits
actions = ticker.actions
print("\nStock Actions:")
print(actions)

Output
https://github.com/dwaynewebb86/y-finance-module/blob/a733fb28472953c33ae3bcd8d44a5f6143bafe5f/yfinance.png
