# Bollinger Band Filters

Only zones touching Bollinger Bands:

This filter checks whether any candle between the start and end of the zone is touching, breaking or outside of the upper or lower Bollinger band. In the case of a demand zone, it must be the lower Bollinger Band, whilst for a supply zone it must be the upper Bollinger band. The standard deviation and moving average for the Bollinger Band default to 2.0 and 20 respectively, but may  changed as required.

The following charts illustrate how this parameter filters out zones. The first chart shows the picture without any filtering applied.

![](/assets/bbfilter1.png)

In the next chart, we see many of the zones fade into the background. From observation, we see that the zones with thin lines are those that were fully inside the Bollinger Bands at the time they were formed. As you can see, it only takes a single wick of one candle to be outside the Bollinger bands in order for the zone to remain active. This filter is best used when you are interested in retests that happen soon after the zone has formed. This is because the position of the zone in terms of Bolilnger bands becomes less relevant as time passes. 

![](/assets/bbfilter2.png)









