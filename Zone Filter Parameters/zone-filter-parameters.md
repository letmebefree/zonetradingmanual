# Zone Filter Parameters

The following criteria are unique to zones and can be used to set the as active or in-active. By default, inactive zones will appear with thinner lines on a chart \(can also be set to disappear completely\) and will not be considered for setting orders when the EA is placed in auto-trading mode.

**Maximum prior retests of zone:**

For each possible zone on the chart, the EA counts the number of times that price has left the zone and then come back to retest it. If the count is greater than the value of this parameter, the zone will be made inactive, For example if price has left and then returned to retest a zone twice, setting the value to 1 or lower will cause the zone to be inactive. The principle is that the more times price has retested a zone, the fewer institutional orders will be remaining to absorb the momentum and create a reversal.

**Maximum zone penetration \(%\):**

This parameter sets a maximum zone penetration allowed by price since the zone first formed. The principle behind this is that the further price has penetrated a zone, the closer it is getting to breaking the stop level. In practice, each zone on the chart probably contains one or more zones from lower time frames. Each of these lower time frame zones will present some resistance to price in the form of institutional orders placed by traders. Each time the zone is retested, orders at each level will be filled. Eventually all orders at all levels within the original zone will be filled and the zone will be broken.

**Maximum zone depth in pips:**

If the distance between the zone entry and stop level is greater than the parameter value supplied, the zone will be made inactive. It is preferable to trade zones with a smaller distance as these typically provider higher Reward to Risk potential and also allow larger positions sizes and therefore bigger potential profits without increasing overall risk exposure.

**Minimum zone depth in pips:**

If the distance between the zone entry and stop level is less than the parameter value supplied, the zone will be made inactive. If a zone is too narrow, there is unlikely to be any additional orders from smaller time frame zones inside and its strength will therefore be diminished.

**Maximum candles since zone formation:**

If the number of candles that have closed since the zone formed is greater than the value specified, the zone will be made inactive. This allows for trading only rapid retests soon after a zone first forms, a useful method for getting into a new trend at the start. For example, when a chart is in an uptrend, you may want to enter on any rapid retracement back to demand that happens within 10 candles of the demand first being created. Setting the value of the parameter to 10 ensures that no orders are entered for this particular zone after 10 candles have completed.

