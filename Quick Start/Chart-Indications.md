# Chart Indications

You will see a number of indicators and labels and charts that it is important to understand.

## Summary Information

In the top left of the chart, you can see the following:

An indication of the current trend for each time frame for which zones are currently being identified.

In the chart below, we see the text ”MN1:U W1:U D1:D H1:D M30:D M15:D”.

Amongst other things, this tells us that the current trend on the W1 chart is up, whilst the trend on the M30 chart is down.

[![](https://github.com/letmebefree/zonetradingmanual/raw/master/assets/chart_indicators.png)](https://github.com/letmebefree/zonetradingmanual/blob/master/assets/chart_indicators.png)

Underneath the trend indicators,, you will see indicators representing the move up and move down for both the current week and the current day. The calculation is performed as follows:

The **daily **moves for the latest candle are calculated every tick, based on whether the closing price of the candle was above \(bullish\) or below \(bearish\) the open price.

For a bullish candle:

* Daily move up = High – Low
* Daily move down = Maximum of: High – Close, Open - Low

For a bearish candle:

* Daily move up = Maximum of: Close – Low, High – Open
* Daily move down = High - Low

The weekly moves for each candle are calculated based on whether the closing price of the candle was above \(bullish\) or below \(bearish\) the open price.

For a bullish candle:

* Weekly up move = High – Low

* Weekly down move = Maximum of: High – Close, Open - Low

For a bearish candle:

* Weekly up move = Maximum of: Close – Low, High – Open
* Weekly down move = High - Low

## Zones

Zones are represented by two lines on a chart, one \(closest to price\) being the entry level and the other \(furthest from price\) being the stop level. Whilst the entry level is a solid line, the stop level is a dashed line.

Once price has passed through a zone, that zone is considered invalid as there can no longer be any pending orders remaining in the zone to be filled. The zone is therefore no longer considered by the EA, will not be displayed on the chart.

In contrast, inactive zones have not yet been invalidated \(stopped out\), but have been excluded from consideration for trading purposes due to not meeting criteria for the strategy. However, inactive zones are still by default represented on a chart by thinner lines than those used for active zones \(this may be changed through parameters\)

Its important to remember that invalid zones will never be displayed or used by the EA, but inactive zones will not be considered for possible trades but are still used for calculations such as distance to next opposing zone and the derivation of a price curve. They may also be displayed on the chart, typically with thinner lines than active zones to differentiate them. It is possible to control the line widths, or prevent zones from being drawn at all using the EA display parameters.

On price charts, zones are colour coded based on the time frame that they are derived from. The colours used for each time frame are as follows:

* MN1 – Green
* W1 – Blue
* D1 – Red
* H4 – Purple
* H1 – Magenta \(Pink\)
* M30 – Orange
* M15 – Lime \(Light Green\)
* M5 – Aqua \(Light Blue\)
* M1 – Yellow

At the start or each line, you will notice a D or S followed by a number. The number represents the previous retests of the zone, whilst the D/S indicate if the zone is supply or demand.

