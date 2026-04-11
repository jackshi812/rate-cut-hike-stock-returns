# Interest Rate Regime Analysis (Rate Cuts vs Hikes)

## Overview
This project analyzes how financial markets respond to changes in monetary policy, specifically interest rate hikes and cuts. Using historical macroeconomic and market data, the goal is to quantify the impact of rate decisions on asset returns and volatility.

## Dataset
- Federal Reserve rate decisions (FOMC)
- Market data (equities, bonds, or sector indices)
- Macroeconomic indicators (optional)
- Time period: Historical time series aligned with rate events

## Methodology

### Data Processing
- Cleaned and aligned time series data across sources  
- Created event indicators for rate hikes, cuts, and neutral periods  
- Engineered features such as returns, volatility, and lagged variables  

### Modeling Approach
- Event study framework to measure abnormal returns around rate changes  
- Regression models (OLS / panel regression) to estimate sensitivity  
- Optional: GARCH models to capture volatility dynamics  

### Evaluation
- Compare market behavior during:
  - Rate hike periods  
  - Rate cut periods  
- Analyze differences in:
  - Returns  
  - Volatility  
  - Sector-level sensitivity  

## Key Results
- Rate hikes are typically associated with lower equity returns and higher volatility  
- Rate cuts often signal economic slowdown but can support market recovery  
- Sensitivity varies significantly across sectors and asset classes  

## Business / Investment Insight
- Helps investors adjust portfolio allocation based on monetary policy cycles  
- Provides a framework for timing risk exposure  
- Supports macro-driven trading and risk management strategies  

## How to Run
1. Clone the repository  
2. Install dependencies:
   pip install -r requirements.txt  
3. Run notebooks:
   jupyter notebook notebooks/

## Tech Stack
- Python (pandas, numpy, statsmodels, scikit-learn)  
- Time Series Analysis  
- Econometrics (OLS, panel regression, GARCH)  

## Future Improvements
- Incorporate high-frequency event windows (intraday data)  
- Extend to global central banks (ECB, BOJ)  
- Apply machine learning models for regime classification  
- Backtest trading strategies based on rate signals  
