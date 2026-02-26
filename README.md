# Trader-Performance-vs-Market-Sentiment

This project creates simple visual charts from Hyperliquid historical trading data and prepares the data for further analysis such as win-rate, PnL trends, and trading behavior.
All the code are done inside jupyter notebook.
In this project we have used python Pandas library for data transformtion and Matplotlib for visualization.
To run this code first save csv file and code file in same folder. Then start running the code.

Summary :-
We analyzed the historical trading dataset (`historical_data.csv`) using Python, pandas, and matplotlib.  
Each trade timestamp was converted from milliseconds to a daily date level.  
The analysis focused on simple, interpretable metrics created directly from the raw trade data:

- daily number of trades (trading activity),
- daily total PnL and daily average PnL per trade,
- daily win rate (Closed PnL > 0),
- daily average trade size (used as a proxy for risk / leverage),
- daily long and short trade counts (directional bias).

Where required, the following assumptions were used:
- A trade is considered a win if `Closed PnL > 0`.
- Average trade size (USD) is treated as a proxy for leverage because explicit leverage data is not available in the dataset.

The analysis is purely descriptive and intended to uncover behavior patterns rather than build a predictive model.
