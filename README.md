# primetrade-sentiment-analysis
# Trader Performance vs Market Sentiment Analysis

## Overview

This project analyzes the relationship between market sentiment (Fear vs Greed) and trader behavior/performance using historical trading data from Hyperliquid and the Bitcoin Fear & Greed Index. The objective is to identify behavioral patterns, evaluate trader performance under different market conditions, and derive actionable trading strategies.

---

## Dataset Description

### 1. Bitcoin Market Sentiment Dataset

* Features: Date, Fear & Greed Value, Classification (Fear/Greed)
* Purpose: Provides daily market sentiment indicators.

### 2. Historical Trader Data (Hyperliquid)

* Features include:

  * Account
  * Coin
  * Execution Price
  * Size USD
  * Side
  * Timestamp
  * Closed PnL
  * Fee
  * Trade ID
  * Transaction Details

---

## Methodology

### Data Preparation

* Loaded and inspected both datasets.
* Checked for missing values and duplicate records.
* Converted timestamps to datetime format.
* Created a common daily date field.
* Merged trader data with market sentiment data.

### Feature Engineering

The following metrics were generated:

* Daily Profit & Loss (PnL)
* Daily trades count
* Trader win rate
* Average trade size
* Long/Short ratio
* Trader frequency segments
* Winner consistency categories

### Analysis Performed

* Compared trader performance during Fear vs Greed periods.
* Analyzed changes in trading behavior based on sentiment.
* Segmented traders into behavioral groups:

  * Frequent vs Infrequent traders
  * Consistent vs Inconsistent winners
  * Large vs Small position traders

---

## Key Insights

1. Trader behavior varies across market sentiment conditions, indicating that market psychology influences trading decisions.

2. The majority of traders are inconsistent performers, while only a small number maintain consistently high win rates.

3. Trading frequency alone does not guarantee profitability, suggesting that trade quality is more important than trade quantity.

4. Position preferences (buy/sell behavior) differ between Fear and Greed market conditions.

---

## Strategy Recommendations

### Strategy 1: Fear Market Risk Management

During Fear periods, traders should reduce position sizes and avoid excessive trading to minimize risk exposure.

### Strategy 2: Selective Participation During Greed

During Greed periods, traders with historically strong performance should increase participation while maintaining disciplined risk management.

### Strategy 3: Quality-Driven Trading

Traders should prioritize trade quality and consistency over increasing trade frequency.

---

## Repository Structure

├── Primetrade_Assignment.ipynb
├── README.md
├── requirements.txt
└── outputs/
    ├── charts
    ├── tables
    └── csv outputs

---

## Installation

Install the required libraries.

## How to Run

1. Clone the repository.
2. Install the required dependencies.
3. Open the Jupyter Notebook:

   ```
   jupyter notebook
   ```
4. Run all cells in `Primetrade_Assignment.ipynb`.
5. Generated charts and tables will be stored in the `outputs` folder.

---

## Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Conclusion

This analysis demonstrates that market sentiment significantly influences trader behavior and performance patterns. Behavioral segmentation and sentiment-aware strategies can help improve decision-making and risk management in cryptocurrency trading.
