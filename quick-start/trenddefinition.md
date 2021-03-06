# Trend Definition

Trend can be defined in many different ways by different traders. It is very hard to find a consistent definition However, when using zones a very specific, consistent and repeatable approach is required.

Two different trend definitions have been implemented for use within the EA.

* TREND\_BY\_ZONE - The trend is determined according to the last zone touched by price
* TREND\_BY\_MA - The trend is determined by relative position of a 10 period EMA and a 12 period SMA 

The preferred choice can be selected by changing the shared parameter "Method for calculating bias trends"

TREND\_BY\_ZONE

The principle used by the EA is that imbalances between supply and demand create price movement, which in turn dictate the direction of the trend. This raises the question of whether trend is necessary to determine future price movement, or if trend is simply the consequence of supply and demand across multiple time frames producing a net movement on price?

For purposes of trading supply and demand, the definition of trend is kept simple. When price last touched or created a supply zone, then the trend is typically down. Conversely, when price last touched or created a demand zone, then the trend would typically be up. However, any zones where a candle has opened or closed between the zone stop and entry will not be included in this determination. In this scenario, it is considered that the zone has considerably weakened and is unlikely to create a reversal in trend.

This approach for determining trend is based on the idea that supply creates a downward pressure on price, whilst demand creates an upward pressure on price. When price has just left an area of supply, it must be moving lower and will continue to do so until the effects of demand start reducing the imbalance of buy and sell orders. Likewise, when price has just touched demand, price movement or trend will change to up and will continue to be so until the imbalance of buy and sell order reverses once again. This continual changing of direction of trend is what causes price to move in waves as it progresses in the direction of a higher time frame trend.

The EA does not particularly consider such a thing as a sideways move, preferring to consider it as a series of alternate up and down trends, where price is trapped between supply and demand zones on the higher time frame.

Of course, price movement is not just based on supply on supply and demand from a single time frame, but the resulting net effect from zones across multiple time frame. This is why it becomes so important to understand what is happening across all time frames, in particular those longer term ones. One of the key benefits of Zone-Trader tutor is that it helps you do this much more quickly and effectively.

TREND\_BY\_MA

This gives a more traditional indication of which way price is moving, looking at the relative positions of a fast exponential moving average and a slower simple moving average. The periods in use default to 10 and 12 respectively. However, these can be changed using parameters.

If the faster moving EMA is above the slower moving SMA, then the trend is considered up . If the relative positions are reversed, the trend is considered down

My own preference is to use TREND\_BY\_ZONE as I work on the basis that trend is determined by zones and therefore we should not be using trends to determine which zones to trade off. In addition, during ranging periods, the traditional trend indicator that lags actual price movement can be somewhat unreliable.

However, the TREND\_BY\_MA is a more traditional definition of trend and many traders would want only want to trade in the direction of this trade on a higher time frame such as the weekly chart.

![](../.gitbook/assets/h4trenddefintions.JPG)

