# About Zone-Trader

Zone-Trader is an expert adviser (or trading robot) written for the MT4 or MT5 trading platforms. It's underlying approach is to identify zones of supply and demand across different time frames and represent these in a way that allows traders to quickly identify when to buy, when to sell and when to stay out of the market. 

Identified supply and demand zones can be manually filtered according to a large number of parameters associated with either the zone itself, or the time when price comes back to retest the zone. The former includes values such as the depth of zone, penetration of the zone at the last retest, number of prior retests of the zone, or distance to the next opposing zone on the same time frame. In contrast, parameters associated with the time when price comes back to retest the zone include the hour of the day, the day of the week, position of price relative to a moving average, an RSI value, or the number of completed consolidation candles. All time based parameters are associated with a specific time frame. 

By selecting multiple criteria to filter zones, we can consider only those zones thought to be high probability trading opportunities. A simple example of applying criteria to filter zones is to include only those where trades taken on retests would be in line with the current trend as of the time of retest, which have a depth of less than 50 pips.

Understanding how each of these parameters impact the overall probability of a trading opportunity achieving its goal is the key to success with this approach. Therefore Zone=Trader provides back testing functionality that enables detailed analysis of supply and demand across different time frames and currencies with filtering criteria being applied in many different ways. Results can be seen instantly on charts or extracted to files for more detailed analysis.

When a configuration of parameters (strategy) has been designed for the given market conditions, the next step is to trade the strategy consistently. To facilitate this, Zone-Trader provides an auto-trading capability.After successful back testing its possible to just turn on auto-trading and let the strategy be traded unattended.

Short and long term strategies can be traded simultaneously by simply setting up the EA on different charts and changing the unique identifier for each instance of the expert adviser.
