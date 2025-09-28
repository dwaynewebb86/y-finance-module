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

dat = yf.Ticker("MSFT")

One ticker symbol
-----------------
dat = yf.Ticker("MSFT")

dat.info

dat.calendar

dat.analyst_price_targets

dat.quarterly_income_stmt

dat.history(period='1mo')

dat.option_chain(dat.options[0]).calls

Multiple ticker symbols
-----------------------
tickers = yf.Tickers('MSFT AAPL GOOG')

tickers.tickers['MSFT'].info

yf.download(['MSFT', 'AAPL', 'GOOG'], period='1mo')

Funds
-----
spy = yf.Ticker('SPY').funds_data

spy.description

spy.top_holdings
