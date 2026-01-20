# PrimeTrade: Trader Performance vs Market Sentiment (Fear & Greed Index)

## Overview
This project analyzes the relationship between Bitcoin market sentiment (Fear & Greed Index) and trader performance using Hyperliquid historical trading data.

## Datasets Used
1. **Fear & Greed Index Dataset**
   - Columns: `date`, `classification`, `value`, `timestamp`

2. **Hyperliquid Historical Trader Dataset**
   - Columns: `Account`, `Coin`, `Execution Price`, `Size USD`, `Side`, `Timestamp IST`, `Closed PnL`, `Fee`, etc.

## Key Steps
- Converted trade timestamps into daily dates
- Merged trade data with daily sentiment data
- Computed **NetPnL = Closed PnL - Fee**
- Performed sentiment-wise analysis:
  - Average NetPnL
  - Total NetPnL
  - Win rate
  - BUY vs SELL behavior

## Outputs
- Sentiment-wise performance summary table
- Bar charts for:
  - Average NetPnL vs Sentiment
  - Win Rate vs Sentiment
  - BUY vs SELL percentage by sentiment

## How to Run
1. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib
