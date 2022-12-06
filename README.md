# Manage-Your-Investment-Portfolio-Part-3
This is a part 3 series of elementary finance analysis using Python 

As opposed to other two parts, part 3 provides an analysis of a cryptocurrency portfolio by using live continuous data. The latter is repeatedly updating (every second), providing an investor with real-time information about the investment performance.

## Breakdown of the file:

Cell 1 → Libraries that are used in the code are imported. 

Cell 2 → The connection to Binance API is established via “Client” module. Therefore, API key is required (account at Binance – see the code for instructions). Additionally, cryptocurrency (e.g. “BTCUSDT”) is defined here. 

Cell 3 → Data is retrieved from API and stored in a DataFrame via “get_historical_klines” (see Binance API docs). The amount of BTC and money invested (USD) are defined and based on that, other data is generated. 

Cells 4, 5 and 6 →  Similar lines of code as in the other two parts (data visualization). Data retrieval intervals (1 sec) and past time (2h from the moment the code is run) are defined in a function “animate”. In an object “ani”, an animation module (FuncAnimation is imported) is used for the purpose of visualizing an interactive chart. 
