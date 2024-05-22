# AI Powered Trading Bot

This repository contained an AI-powered trading bot designed to operate with complete automation, leveraging sophisticated machine learning models and algorithms to make trading decisions. The project demonstrated the potential of algorithmic trading, similar to strategies employed by prominent hedge funds like Renaissance Technologies and Two Sigma.

## Purpose

The primary purpose of this project was to build a fully automated trading bot capable of making profitable trades using AI and machine learning. The bot was designed to:
- Implement advanced trading algorithms.
- Use machine learning models to analyze market sentiment.
- Backtest trading strategies using historical data.
- Manage position sizing and risk dynamically.

## Project Structure

The project was structured into several key components:

### 1. Baseline Bot

- **Initial Setup**: Created the foundational structure for the trading bot, including setting up API connections and importing necessary libraries.
- **Dependencies**: Utilized the `lumot` library to provide a trading framework, including components for brokers, data backtesting, and trading strategies.

### 2. API Integration

- **Alpaca API**: Integrated with the Alpaca trading API to execute trades. Configured API keys and connected to the Alpaca brokerage platform.
- **Data Retrieval**: Used the Yahoo Finance API for backtesting historical data and obtaining real-time data for live trading.

### 3. Trading Strategy

- **Strategy Class**: Developed a custom trading strategy class, `MLTrader`, inheriting from the `Strategy` class provided by the `lumot` library.
- **Lifecycle Methods**: Implemented lifecycle methods such as `initialize` for setup and `on_trading_iteration` for executing trades based on new data.

### 4. Position Sizing and Risk Management

- **Dynamic Position Sizing**: Calculated position sizes dynamically based on available cash and risk tolerance.
- **Risk Management**: Implemented mechanisms to set take profit and stop loss limits to manage trading risks effectively.

### 5. Sentiment Analysis

- **News Data Integration**: Integrated a method to fetch recent news articles relevant to the trading symbols.
- **Sentiment Model**: Applied a pre-trained sentiment analysis model (FinBERT) to determine the sentiment of the news articles.
- **Sentiment-Based Trading Decisions**: Incorporated sentiment analysis results into trading decisions, allowing the bot to trade based on positive or negative market sentiment.

### 6. Backtesting Framework

- **Backtesting Setup**: Configured a backtesting environment using historical data to evaluate the performance of the trading strategy.
- **Performance Metrics**: Analyzed key performance metrics such as cumulative returns, compound annual growth rate (CAGR), and other relevant statistics to assess the effectiveness of the strategy.

## Results

- **Performance Analysis**: The trading bot showed promising results with significant returns over the backtested period, though it also highlighted the challenges of transitioning from paper trading to live trading, including the impact of commissions and fees.
- **Trade Logs**: Included detailed trade logs and performance metrics to allow further investigation and validation of the trading strategy.

## Conclusion

This AI-powered trading bot project provided a comprehensive demonstration of how machine learning and algorithmic trading techniques could be combined to create an automated trading system. The repository included all necessary components, from initial setup and strategy development to sentiment analysis and backtesting, offering a robust foundation for further exploration and enhancement in the field of algorithmic trading.
