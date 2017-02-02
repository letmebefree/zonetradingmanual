# Zone Filter Parameters

The following criteria are unique to zones and can be used to set the as active or in-active. By default, inactive zones will appear with thinner lines on a chart \(can also be set to disappear completely\) and will not be considered for setting orders when the EA is placed in auto-trading mode.

**Trading Bias**

The trading bias is used to filter out zones which are counter the trend for an associated time frame. The time frame and direction may be set manually or calculated by the Expert Adviser according to the selected parameter value.

Up to four different biases can be applied. For example, if the bias for the H1 time frame should be up when the trend on the D1, W1 and MN1 time frames are also up, or down when the trend on the D1, W1 and MN1 time frames are also down, each of three different bias settings can be applied using values of BIAS\_D1\_TREND, BIAS\_W1\_TREND and BIAS\_MN1\_TREND respectively. In this scenario, if any of the trends in these three higher time frames are different from the others, there will be no active zones on the H1 chart.

Descriptions for each possible setting are given below:

BIAS\_NONE

Across all time frames, no bias will be set and both supply and demand zones will be displayed as active

BIAS\_UP

Across all time frames, only demand zones will be displayed as active on the chart

BIAS\_DOWN

Across all time frames, only supply zones will be displayed as active on the chart

BIAS\_HTF\_TREND

The bias for each time frame will be set according to the trend on the next higher time frame. For example, if the trend on the D1 chart is up, only demand zones will be active on the H4 chart. Similarly, if the trend on the H1 chart is down, only supply zones will be active on the M30 chart. A bias on the MN1 chart will not be set as there is no available higher time frame

BIAS\_HHTF\_TREND

The bias for each time frame will be set according to the trend from two time frames higher. For example, if the trend on the W1 chart is down, then only supply zones will be shown as active on the H4 chart. Similarly, if the trend on the MN1 chart is up, only demand zones will be active on the D1 chart. The bias on the MN1 chart will not be set.

BIAS\_H1\_TREND

The bias for each time frame smaller than the H1 time frame will be set according to the trend from the H1 time frame. For example, if the trend on the H1 chart is down, then only supply zones would remain active on the M30, M15, M5 and M1 charts.

As it makes no sense to set a bias for timeframes equal or higher than H1, these will be left with no bias applied \(both supply and demand zones will remain active\).

BIAS\_H4\_TREND

The bias for each time frame smaller than the H4 time frame will be set according to the trend from the H4 time frame. For example, if the trend on the H4 chart is down, then only supply zones would remain active on the H1, M30, M15, M5 and M1 charts.

As it makes no sense to set a bias for timeframes equal or higher than H4, these will be left with no bias applied \(both supply and demand zones will remain active\).

BIAS\_D1\_TREND

The bias for each time frame smaller than the D1 time frame will be set according to the trend from the D1 time frame. For example, if the trend on the D1 chart is down, then only supply zones would remain active on the H4, H1, M30, M15, M5 and M1 charts.

As it makes no sense to set a bias for timeframes equal or higher than D1, these will be left with no bias applied \(both supply and demand zones will remain active\).

BIAS\_W1\_TREND

The bias for each time frame smaller than the W1 time frame will be set according to the trend from the W1 time frame. For example, if the trend on the W1 chart is down, then only supply zones would remain active on the D1, H4, H1, M30, M15, M5 and M1 charts.

As it makes no sense to set a bias for timeframes equal or higher than W1, these will be left with no bias applied \(both supply and demand zones will remain active\).

BIAS\_MN1\_TREND

The bias for each time frame smaller than the MN1 time frame will be set according to the trend from the MN1 time frame. For example, if the trend on the MN1 chart is down, then only supply zones would remain active on the W1, D1, H4, H1, M30, M15, M5 and M1 charts.

As it makes no sense to set a bias for timeframes equal or higher than MN1, these will be left with no bias applied \(both supply and demand zones will remain active\).

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

