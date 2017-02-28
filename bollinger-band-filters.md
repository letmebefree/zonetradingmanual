# Bollinger Band Filters

Only zones touching Bollinger Bands:

This filter checks whether any candle, between the start of the zone and the time when it first formed, is touching, breaking or outside of the upper or lower Bollinger band. In the case of a demand zone, it must be the lower Bollinger Band, whilst for a supply zone it must be the upper Bollinger band. The standard deviation and moving average for the Bollinger Band default to 2.0 and 20 respectively, but may  changed as required.

The following charts illustrate how this parameter filters out zones. The first chart shows the picture without any filtering applied.

![](/assets/bbfilter1.png)

In the next chart, the circle marked "1" shows where a wick from a zone means it remains active.  In the circle marked '2' none of the candles at zone creation protrude ouside the Bollinger bands so the zone is set inactive. 

The idea behind this is that the active zones occurred when price was stretched away from the moving average. Therefore, the probability is that not everyone managed to get into the trade as price reverted back to the mean. The retest gives them  the opportunity to enter the market at this same level. 

This filter is best used when for retests that happen soon after the zone has formed. Beyond this scenario, the position of the zone in terms of Bollinger bands becomes less relevant as time passes. Or put another way, traders are less interested in an area where price may no longer be classed as ready to revert back to the mean.

![](/assets/bollinger2.png)

