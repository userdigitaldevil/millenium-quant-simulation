# Millenium Quant Trader Assessment Solution

This repository contains my solution for the Millenium quant trader assessment.

## Overview

The assessment solution is implemented in the Jupyter notebook `millenium-quant-assessment-solution.ipynb`, which contains a comprehensive implementation of quantitative trading strategies and market making algorithms. The notebook is structured as a progressive learning experience that builds from basic market making to advanced arbitrage trading.

## Notebook Contents

### **Challenge 1: Price Making & Market Making Fundamentals**
- **Task A**: Data preparation and sample dataset creation from price requests
- **Task B**: Reference price matching and data structure creation
- **Task C**: Implementation of `QuotedTrade` class with bid/offer price calculations using 2% spread
- **Task D**: Hedge fund interaction and trade decision processing
- **Task E**: Market maker initialization and position tracking
- **Task F**: Quote logging and trade management
- **Task G**: `CompletedTrade` class implementation for executed trades
- **Task H**: Position updates and trade completion logging
- **Task I**: Data visualization of AAPL quotes over time using matplotlib

### **Challenge 2: Risk-Based Price Skewing & Advanced Market Making**
- **Task A**: Implementation of risk-based skewing algorithm that adjusts bid/offer prices based on current inventory positions
- **Task B**: Visualization of skewed quotes showing how prices are adjusted for risk management
- **Key Features**: 
  - Long position management (encouraging buyers)
  - Short position management (encouraging sellers)
  - Neutral position handling with symmetric spreads

### **Challenge 3: Beta-Adjusted ETF Hedging Strategy**
- **Research Section**: Beta calculation for 5 FAANG stocks relative to FAANG ETF
  - AAPL: β = 0.865, FB: β = 1.032, GOOGL: β = 1.269, AMZN: β = 0.919, NFLX: β = 0.921
- **Task A**: Implementation of beta-adjusted hedging algorithm using `ExchangeTrade` class
- **Task B**: Risk exposure visualization showing total net position over time
- **Key Features**: 
  - Beta-based hedge ratio calculations
  - Automated ETF position management
  - Risk exposure tracking and visualization

### **Challenge 4: Arbitrage Trading & Statistical Arbitrage**
- **Research Section**: Arbitrage opportunity identification between real FAANG ETF and synthetic ETF
- **Task A**: Complete arbitrage algorithm implementation with entry/exit signals
- **Key Features**:
  - Z-score based entry/exit signals (entry at |Z| ≥ 2.0, exit at |Z| ≤ 0.5)
  - Multi-leg trade execution (ETF + 5 component stocks)
  - Commission-aware profit calculations
  - Position flattening and risk management

### **Technical Implementation Details**
- **Object-Oriented Design**: Custom classes for `QuotedTrade`, `CompletedTrade`, and `ExchangeTrade`
- **Data Processing**: Pandas DataFrame operations for time series analysis
- **Risk Management**: Position tracking, skewing algorithms, and hedging strategies
- **Visualization**: Matplotlib charts for price analysis, risk exposure, and arbitrage opportunities
- **Trading Logic**: State machine implementation for arbitrage strategy with regime tracking

### **Key Algorithms & Strategies**
1. **Market Making**: 2% spread calculation with risk-based price skewing
2. **Beta Hedging**: Statistical hedge ratio calculation using covariance/variance analysis
3. **Statistical Arbitrage**: Z-score based mean reversion trading between correlated assets
4. **Risk Management**: Position-based price adjustments and automated hedging

## Files

- `millenium-quant-assessment-solution.ipynb` - Main solution notebook containing the assessment implementation

## Getting Started

To run the solution:

1. Ensure you have Jupyter Notebook or JupyterLab installed
2. Open the notebook file
3. Run the cells sequentially to execute the solution

## Requirements

The solution may require various Python packages for quantitative analysis. Please refer to the notebook for specific import statements and dependencies.

## Important Note

**Note:** During the simulation, I do not have access to the Amplify Libraries or the actual datasets that would be used in a real assessment environment. The solution is based on the problem description and my understanding of the requirements.

---

_This repository represents my work on the Millenium quant trader assessment._
