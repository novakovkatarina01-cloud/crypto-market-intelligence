# crypto-market-intelligence


## Project Overview

This project builds an end-to-end cryptocurrency market intelligence pipeline using the CoinGecko API, Databricks, PostgreSQL, and Tableau.

The pipeline extracts cryptocurrency market data from the CoinGecko API, performs data transformation and cleaning in Databricks, stores the processed data in PostgreSQL, and visualizes key market insights through an interactive Tableau dashboard. Aditionally automated Crypto ETL Job is created that will automaticaly run everyday once.

## Architecture

CoinGecko API → Databricks ETL → PostgreSQL Database → Tableau Dashboard
## Database Schema

The cleaned cryptocurrency data is stored in a PostgreSQL database (`crypto_market`) in the table `crypto_prices`.

Key fields include:

- id
- symbol
- name
- current_price
- market_cap
- market_cap_rank
- total_volume
- high_24h
- low_24h
- price_change_percentage_24h
- last_updated
- etl_load_timestamp

  ##
  # Databricks Automation

A Databricks Job was configured to automate execution of the ETL notebook.

Job Name: Crypto ETL Job

Purpose:
- Run the ETL pipeline automatically
- Refresh cryptocurrency market data
- Support automated data updates

## Technologies Used

* Python
* CoinGecko API
* Databricks
* PostgreSQL (pgAdmin 4)
* Tableau Public
* GitHub

## Repository Contents

* `01_extract_coingecko.ipynb` – Databricks ETL notebook
* `crypto_prices.csv` – Processed cryptocurrency dataset
* `crypto_market_dashboard 2.twbx` – Tableau dashboard workbook

## Tableau Dashboard

Tableau Public Dashboard:

https://public.tableau.com/app/profile/katarina.novakov3974/viz/crypto_market_dashboard2/CryptocurrencyMarketIntelligenceDashboard

