# SMA Trading Strategy Backtest

This repository contains a backtest implementation of a Simple Moving Average (SMA) trading strategy applied to daily stock data. The strategy is designed to be applied to any stock by changing the ticker name.

## Strategy Overview

- **Ticker**: The strategy is backtested on RELIANCE stock but can be adapted to any stock by updating the ticker name.
- **Trading Signal**:
  - **Buy Signal**: Generated when the 30-day Simple Moving Average (SMA) is above the closing price. The position is opened at the next day’s opening price.
  - **Sell Signal**: Generated when the 30-day SMA is below the closing price. The position is closed at the next day’s opening price.
- **Columns in Output**:
  - `Signals`: 1 for Buy and -1 for Sell.
  - `Entry`: Price at which the position is opened.
  - `Exit`: Price at which the position is closed.
  - `Entry Date`: Date when the position is opened.
  - `Exit Date`: Date when the position is closed.
  - `PercRet`: Percentage return of the trade.

## Performance

The strategy was backtested on RELIANCE stock from 2008 to 2024 and achieved a total return of 225%.

## Usage

1. **Setup**: Clone this repository and navigate to the project directory.

   ```bash
   git clone https://github.com/trippynix/Strategies-Backtesting.git
   cd Strategies-Backtesting

2. **Requirements**: Install the necessary Python packages.

   ```pip install pandas
      pip install numpy
      pip install yfinance

3. **Run Backtest**:

- Modify the ticker symbol in the script to backtest different stocks.
- Run the backtesting script:
   ```python "Simple Moving Average Strategy Backtest on Reliance.ipynb"

4. **Analyze Results**:

- The output includes columns for trading signals, entry and exit prices, entry and exit dates, and percentage returns.
- The performance of the strategy can be reviewed in the output CSV or analyzed within the script.

## Files

- "Simple Moving Average Strategy Backtest on Reliance.ipynb": Python script implementing the SMA strategy.

## Acknowledgements

- Data sourced from NSE for RELIANCE stock.
- Inspired by various trading strategies and backtesting practices.

##FEEL FREE TO MODIFY IT AS NEEDED TO FIT YOUR SPECIFIC PROJECT DETAILS.
