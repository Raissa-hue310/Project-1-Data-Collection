Project 1: Data Collection and Initial Analysis of Stock Market Data
Student: Raïssa Matho Mekjele
Date: November 2025

📁 Project Overview

This project performs a comprehensive exploratory data analysis (EDA) of daily stock market data covering multiple decades (1970–2018). It focuses on building essential data science skills including:

Loading and inspecting large datasets

Cleaning and preparing structured financial data

Segmenting historical data into decades

Visualizing long-term trends in prices and volume

Comparing financial behavior across different historical periods

This foundational analysis prepares for more advanced modeling in subsequent projects (forecasting, volatility modeling, sector-based comparison, etc.).

📂 Dataset Description

The project uses the dataset:
Daily Historical Stock Prices (1970–2018)
Downloaded as a ZIP file containing:

File	Description
historical_stock_prices.csv	Daily open, high, low, close, adjusted close, volume, and ticker
historical_stocks.csv	Metadata: stock name, exchange, sector, industry
Main Columns Used

Date: trading date

Open, High, Low, Close, Adj Close: price information

Volume: number of shares traded

Ticker: stock symbol

Sector, Industry: company classification

🔧 Project Steps
1. Data Loading

Unzipped the dataset in Google Colab

Loaded both CSV files using pandas.read_csv()

Converted the date column to datetime

2. Data Cleaning

Handled missing values:

Numeric columns → filled with median

Sector/industry → filled with "Unknown"

Removed duplicate rows

Ensured proper data types (floats, integers, datetime)

Set date as the DataFrame index

3. Data Enrichment & Segmentation

Added year and decade columns

Merged price data with sector information

Created decade-based subsets for comparison

4. Exploratory Data Analysis

Performed EDA with:

Summary statistics (mean, median, std) by decade

Monthly average close price time series

Volume distribution histograms (with log-scale option)

Box plots for high/low prices

Optimized using sampling to avoid memory crashes in Colab

5. Comparative Insights

Analyzed multi-decade trends:

Rising prices across decades

Increased volatility in later decades

Higher trading volumes with structural changes in markets

Possible links to major economic events

6. Initial Hypotheses for Future Work

Relationship between volume and volatility

Sector-based differences in growth and risk

Crisis effects persisting across multiple years

Structural changes due to technology and globalization

📈 Visualizations Included

Line plots of average monthly closing prices

Histograms of trading volume

Box plots for high and low prices (sampled for performance)

Decade-level statistical comparison tables
 (optional)
