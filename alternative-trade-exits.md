### Alternative Trade Exits

**Close trade when price hits opposing Bollinger Band:**

If set to true, this parameters causes an active buy trade to be closed as soon as the high of the current candle touches the upper Bollinger band. An active sell trade will be closed as soon as the low of the current candle touches the lower Bollinger band. The principle behind this is that the Bollinger band represents a level where price has been over extended away from the moving average due to a strong move away from it. Therefore support or resistance from zones is likely to be move effective and a reversal of sorts is likely.

**Close trade when price hits first MA or BB:**

If set to true, the EA will close a trade as soon as a new candle occurs with its high one side of a moving average or Bollinger band and its open on the other side. One scenario is  used when trades are entered at Bollinger band extremes and you wish to exit the position as soon as price touches the corresponding moving average. A second scenario is when trades are entered close to a moving average and you wish to exit the trade as soon as price returns back to the outer Bollinger band.

The parameters for the BolLinger bands and moving averages are taken from the global settings, defaulting to 20 period and standard deviation of 2.

