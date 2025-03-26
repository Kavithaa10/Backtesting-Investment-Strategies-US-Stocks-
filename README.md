# Backtesting-Investment-Strategies-US-Stocks-

### Importing the Data

#### import pandas as pd

#### 1.	Load and inspect the dataset dji.csv.
### Data Visualization & Returns
#### import matplotlib.pyplot as plt
#### import numpy as np
#### import seaborn as sns
#### plt.style.use("seaborn-v0_8")

### Backtesting a simple Momentum Strategy
### Positions:
#### +1: Investing in DJI (long position)
#### -1: Short Selling DJI (short position)
#### 0: No position (neutral)
### Strategies:
#### -Buy and Hold (Basic Strategy - passive): Initially Investing into DJI and do nothing (Position: +1 on any given day)
#### -Simple Momentum (active Strategy to be tested):
#### a) Investing (+1) into DJI tomorrow if today´s return was positive
#### b) Short selling (-1) DJI tomorrow if today´s return was negative

### Backtesting a simple Contrarian Strategy
#### Strategies:
#### -Buy and Hold (Basic Strategy): Initially Investing into DJI and do nothing (Position: +1 on all days)
#### -Simple Contrarian (Strategy to be tested):
#### a) Short Selling (-1) DJI tomorrow if today´s return was positive
#### b) Investing (+1) into DJI tomorrow if today´s return was negative

### More complex Strategies & Backtesting vs. Fitting

#### Even if a Strategy seems to outperform the basic Strategy, the following issues need to be considered/analyzed as well:
#### •	Backtesting vs. Fitting -> Was the Strategy fitted and optimized on historical data? Forward Testing is required!
#### •	Transaction Costs -> Changing Positions trigger Cost. Include Costs!
#### •	Tax effects -> Changing Positions can trigger (earlier) Tax Payments. Include Taxes!

### Simple Moving Averages
### Strategies:
#### -Buy and Hold (Basic Strategy): Initially Investing into DJI and do nothing (Position: +1 on all days)
#### -SMA Crossover (Momentum) (Strategy to be tested):
#### a) Investing (+1): SMA50 > SMA200
#### b) Short Selling (-1): SMA50 < SMA200
