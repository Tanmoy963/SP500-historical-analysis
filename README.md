S&P 500 Market Trends Analysis (2014-2017)
Overview
This project is an end-to-end data analytics pipeline exploring historical stock market data for S&P 500 companies between 2014 and 2017. The goal of this analysis is to identify major market trends, day-of-the-week trading seasonality, asset volatility, and long-term return on investment (ROI). By transforming raw financial data into an interactive dashboard, this project provides actionable insights for portfolio management and trading strategies.

Dataset
Source: Maven Analytics Data Playground

Description: Historical daily trading data for S&P 500 companies.

Key Variables: Date, Ticker Symbol, Open, High, Low, Close, and Volume.

Tools Used
Python (Pandas): Data extraction, exploratory data analysis (EDA), and data cleaning.

SQL (PostgreSQL / MySQL): Querying relational data, aggregating historical volume, and structuring views for BI integration.

Power BI & DAX: Building an interactive financial dashboard with dynamic measures for cumulative ROI and volatility tracking.

Gamma: Generating a professional presentation deck to communicate key findings to stakeholders.

Steps
Data Loading & Cleaning (Python): * Handled local file path encoding and permission errors.

Standardized column names and converted string dates into correct datetime objects.

Exported a clean, optimized cleaned_sp500.csv file.

Exploratory Data Analysis (Python & SQL):

Grouped and aggregated data to find the dates with the highest overall trading volume.

Extracted weekdays to calculate average trading volume and identify seasonality patterns.

Calculated daily price volatility (High - Low) for individual assets.

Data Visualization (Power BI):

Imported the cleaned dataset and established the data model.

Wrote custom DAX measures to calculate dynamic metrics, such as Cumulative ROI % starting from the earliest selected date.

Designed a professional, interactive dashboard with slicers for year and ticker symbols.

Reporting (Gamma):

Synthesized the technical findings into a high-level presentation tailored for portfolio managers and trading desks.

Dashboard
The Power BI dashboard acts as a financial terminal, allowing users to interact with the data through the following visual components:

Time Series Volume Chart: Tracks daily market volume, highlighting major sell-offs and accumulation days.

Top 10 Volume Treemap: Dynamically filters to show the most actively traded stocks on any specific day.

Seasonality Bar Chart: Displays the average trading volume grouped by the day of the week.

Volatility Tracker: A searchable line chart showing the daily price swings of individual stocks.

Cumulative ROI Area Chart: Visualizes the exact percentage growth of an asset over the selected timeframe.

[Insert a screenshot of your Power BI Dashboard here]

Key Results & Business Insights
The 2015 "Flash Crash": August 24, 2015, saw the highest overall market trading volume, driven by massive panic sell-offs in major equities. On this date, Bank of America (BAC) and Apple (AAPL) were the two most heavily traded stocks.

Trading Seasonality: Across the four-year sample, Fridays consistently experienced the highest average trading volume, likely due to end-of-week options expirations and position adjustments. Mondays saw the lowest average volume.

Price Volatility: Amazon (AMZN) experienced its most volatile trading day on June 9, 2017, with a massive $85.99 swing between its daily high and low.

Top Investment Return: Nvidia (NVDA) was the highest-performing asset in the dataset. An investment made on January 2, 2014, and held until December 29, 2017, yielded an 1120.05% cumulative return.



