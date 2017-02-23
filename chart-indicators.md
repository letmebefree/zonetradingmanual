# Chart Indicators

You will see a number of indicators and labels and charts that it is important to understand.

In the top left of the chart, you can see the following:

An indication of the current trend for each time frame for which zones are currently being identified.

In the chart below, we see the text ”MN1:U W1:U D1:D H1:D M30:D M15:D”.

Amongst other things, this tells us that the current trend on the W1 chart is up, whilst the trend on the M30 chart is down.

![](/assets/chart_indicators.png)

Underneath the trend indicators,, you will see indicators representing the move up and move down for both the current week and the current day. The calculation is performed as follows:

The daily move for the latest candle is calculated based on whether the closing price of the candle was above \(bullish\) or below \(bearish\) the open price.

For a bullish candle:

* Daily move up = High – Low
* Daily move down = Maximum of: High – Close, Open - Low

For a bearish candle:

* Daily move up = Maximum of: Close – Low, High – Open
* Daily move down = High - Low



