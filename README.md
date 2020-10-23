### API_Homework
### Student: Michael De Paula


---
---
---
<p align="center">
 <ins><b>Financial Planner</b><br><ins>
</p>


Here we are creating an application that will provide visual information which will be used to determine financial health. We will develop this information by pulling cryptocurrencies data and ETF data using the following tools:

- Imports required
    - import os
    - import json
    - import requests
    - import pandas as pd
    - from dotenv import load_dotenv
    - import alpaca_trade_api as tradeapi
    - from MCForecastTools import MCSimulation
- APIs [Alpaca Markets API](https://alpaca.markets/) and [Alternative Free Crypto API](https://alternative.me/crypto/api/)
- .concat()
- If conditional statement
- .get_barset()
- Creating Dataframes (.pd)
- Monte Carlos Simulations

The data being pulled are Bitcoin ([BTC](https://www.coinbase.com/price/bitcoin)), Ethereum ([ETH](https://www.coinbase.com/price/ethereum)), iShares Core US Aggregate Bond ETF ([AGG](https://www.google.com/finance/quote/AGG:NYSEARCA)) and SPDR S&P 500 ETF ([SPY](https://www.google.com/finance/quote/SPY:NYSEARCA)). Once this data is pulled we will determine the dollar value of each and .concat() them into a dataframe to then reveal a pie chart that reflects a visual value of each. Using this information we will determine whether the amount of stocks, cryptocurrency and cash are a sufficient amount of savings using an if conditional statement. 
We will then adjust the dataframe for AGG and SPY to determine cumulative returns for the next 30 years using a Monte Carlo Simulation and plotting it with a line plot as well as a distribution bar graph. Finally, once the Monte Carlos Simulation is complete we will provide a retirement analysis and calculate the expected return at 95% lower and upper confidence level based on a $20,000 initial investment.  
