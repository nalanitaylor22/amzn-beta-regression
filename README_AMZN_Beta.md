# Estimating Amazon's Market Beta with Python

A Python notebook that measures how sensitive Amazon's stock is to the overall market, using 15 years of monthly data and an OLS regression.

## What it does

1. Downloads monthly adjusted prices for **Amazon (AMZN)** and the **S&P 500 ETF (SPY)** from Yahoo Finance (2011–2025)
2. Combines the series and calculates monthly returns
3. Visualizes the data: returns over time, growth of a $100 investment, return histogram, and a returns scatterplot
4. Runs an OLS regression of AMZN returns on SPY returns to estimate Amazon's **beta**

## Key results

| Metric | Value |
|---|---|
| Beta (AMZN vs. SPY) | **1.196** |
| 95% confidence interval | 0.953 to 1.439 |
| R-squared | 0.349 |
| Observations | 178 monthly returns (Feb 2011 – Nov 2025) |

**What this means:** Amazon has historically moved about 1.2x as much as the market. When the S&P 500 rises or falls 1%, Amazon tends to move about 1.2% in the same direction. The market explains roughly 35% of Amazon's monthly return variation, with the rest driven by company-specific factors. Beta is a key input in the CAPM for estimating a company's cost of equity.

## Tools

Python · pandas · yfinance · matplotlib · statsmodels · Google Colab

## How to run

Open the notebook in Google Colab and run all cells. The required packages install automatically in the first code cell.

---
Built as part of my finance coursework at the University of South Florida.
Nalani Taylor · [LinkedIn](https://www.linkedin.com/in/nalani-taylor-ab582a316)
