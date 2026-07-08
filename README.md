# Data-Science-Intern-project-
# Bitcoin Market Sentiment vs Trader Performance Analysis

## Overview

This project analyzes the relationship between Bitcoin market sentiment and trader performance. The analysis combines a Fear & Greed Index dataset with historical trading data to understand how market sentiment influences profitability, trading behavior, and risk-taking.

## Objectives

* Merge trader activity data with daily market sentiment data.
* Compare trader performance during Fear and Greed market conditions.
* Analyze changes in trading behavior across different sentiment phases.
* Segment traders based on leverage, activity, and consistency.
* Generate actionable trading insights based on the findings.

## Datasets

### 1. Fear & Greed Index Dataset

Contains:

* Daily sentiment classification (Fear, Greed, Extreme Fear, Extreme Greed)
* Fear & Greed score
* Date information

### 2. Historical Trader Dataset

Contains:

* Account information
* Trade direction (Long/Short)
* Position size
* Trade timestamp
* Profit and Loss (PnL)
* Trading fees and other trade details

## Data Preparation

The following preprocessing steps were performed:

1. Loaded both datasets into Python.
2. Converted timestamp columns into datetime format.
3. Extracted the date from trade timestamps.
4. Merged both datasets using the date field.
5. Assigned daily market sentiment to every trade record.

## Feature Engineering

The following metrics were created:

* Daily PnL per trader
* Win Rate
* Average Trade Size
* Number of Trades per Day
* Long/Short Ratio
* Estimated Leverage
* Drawdown Proxy

## Analysis

### Performance Analysis

Compared trader performance between Fear and Greed periods using:

* Average PnL
* Total PnL
* Win Rate
* Drawdown Proxy

### Behavior Analysis

Analyzed whether traders change behavior based on sentiment by studying:

* Trading frequency
* Position sizes
* Leverage usage
* Long vs Short preferences

### Trader Segmentation

Traders were grouped into:

* High-Leverage vs Low-Leverage Traders
* Frequent vs Infrequent Traders
* Consistent vs Inconsistent Traders

## Visualizations

The project includes charts for:

* Average PnL by Market Sentiment
* Win Rate by Market Sentiment
* Average Trade Size by Sentiment
* Long vs Short Distribution
* Daily Trading Activity
* Leverage-Based Performance Comparison

## Key Findings

* Trader performance differed between Fear and Greed periods.
* Traders tended to increase activity and position sizes during Fear periods despite weaker performance.
* Greed periods generally showed stronger profitability and higher win rates.
* Infrequent traders often achieved better average performance than highly active traders.

## Actionable Recommendations

### Strategy 1: Adjust Leverage Based on Market Sentiment

* Reduce leverage during Fear periods.
* Use leverage more cautiously during favorable market conditions.

### Strategy 2: Trade More Selectively During Fear

* Reduce trading frequency during Fear periods.
* Increase activity only when sentiment and performance metrics support it.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Google Colab

## Project Structure

```text

│   ├datasets are direclty loaded from a sharable link.
│
├
│    Task.ipynb
│
├── charts/
│   └── generated_visualizations
│
├── README.md
└── requirements.txt
```

## Conclusion

This project demonstrates how market sentiment can influence trader behavior and performance. By combining sentiment indicators with trading data, traders and analysts can better understand market psychology and develop more informed risk-management strategies.
