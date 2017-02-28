# Auto-trading Parameters

The following parameters are applicable only when the EA is in auto-trading mode

**Timeframe for placing trades:**

Only zones from the specified time frame will be used for creating new limit orders during auto-testing

**Target type for orders:**

This determines how an initial trade target is calculated by the EA at the time of placing the order, also making use of the parameter "Target type value".  The following is a list of possible values for the target type.

TARGET\_NONE

No target will be calculated. Either the trade will be closed manually or the EA will close the trade based on price action or using a trailing stop of some description

TARGET\_FIXED\_R

The target will be calculated as a multiple of the number of pips between the order entry and the stop loss position. This is calculated based on the value of the Target type value. For example, if the stop is 20 pips away from the entry and "Target type value" is 2, then the target will be 40 pips from the entry.

TARGET\_FIXED\_PIPS

The target will be a fixed number of pips away from the order entry, the number of pips being determined by "Target type value".

TARGET\_FIXED\_PRICE

The target will be the same as the price entered against the parameter Target type value.

TARGET\_NEXT\_H1\_ZONE

The target will be set to be the entry price for the next opposing zone on the H1 time frame. For example, for if a pending sell order is being placed, the target will be the entry level for the closest demand zone on the H1 chart. This considers any zone that has not yet been stopped out, not just those that meet the current strategy’s criteria.

TARGET\_NEXT\_H4\_ZONE

The target will be set as the entry price for the next opposing zone on the H4 time frame. For example, if a pending sell order is being placed, the target will be the entry level for the closest demand zone on the H4 chart. This considers any zone that has not yet been stopped out, not just those that meet the current strategy’s criteria.

TARGET\_NEXT\_D1\_ZONE

The target will be set as the entry price for the next opposing zone on the D1 time frame. For example, if a pending sell order is being placed, the target will be the entry level for the closest demand zone on the D1 chart. This considers any zone that has not yet been stopped out, not just those that meet the current strategy’s criteria.

TARGET\_NEXT\_W1\_ZONE

The target will be set as the entry price for the next opposing zone on the H1 time frame. For example, if a pending sell order is being placed, the target will be the entry level for the closest demand zone on the W1 chart. This considers any zone that has not yet been stopped out, not just those that meet the current strategy’s criteria.

TARGET\_NEXT\_CTF\_ZONE

The target will be set as the entry price for the next opposing zone on the same time frame \(the Current Time Frame\) as the zone which is being used to set the order entry. For example, for a pending sell order being placed at a H1 zone, the target will be the entry level for the closest demand zone on the H1 chart. This considers any zone that has not yet been stopped out, not just those that meet the current strategy’s criteria.

TARGET\_NEXT\_HTF\_ZONE

The target will be set as the entry price for the next opposing zone on the next higher time frame to that of the zone being retested. For example, for a pending sell order being placed at a H1 zone, the target will be the entry level for the closest demand zone on the H4 chart. This considers any zone that has not yet been stopped out, not just those that meet the current strategy’s criteria.

TARGET\_DAILY\_MOVE\_REMAINING

The target will be set based on an average of the previous daily up and down price moves.

The daily move for each candle is calculated as follows, based on whether the closing price of the candle was above \(bullish\) or below \(bearish\) the open price.

For a bullish candle:

* Daily move up = High – Low
* Daily move down = Maximum of: High – Close, Open - Low

For a bearish candle:

* Daily move up = Maximum of: Close – Low, High – Open
* Daily move down = High - Low

The average move up and average move down for the previous nine daily candles are calculated. These are then compared with the current daily moves up and down to find the remaining potential move available for the day.

If the retested zone is supply, the target is set as the entry level minus the remaining move down available. If the retested zone is demand, the target is set as the entry level plus the remaining move up available.

If either the daily move up, or daily move down, have already exceeded the value specified in the parameters, the target required would be a move in the opposing direction, which makes no sense. Therefore, before placing an order, the distance between the target and entry will be tested and no order will be placed if it is less than or equal to zero.

TARGET\_WEEKLY\_MOVE\_REMAINING

The target will be set based on an average of previous weekly up and down moves.

The weekly move for each candle is calculated based on whether the closing price of the candle was above \(bullish\) or below \(bearish\) the open price.

For a bullish candle:

* Weekly move up = High – Low
* Weekly move down = Maximum of: High – Close, Open - Low

For a bearish candle:

* Weekly move up = Maximum of: Close – Low, High – Open
* Weekly move down = High - Low

The average move up and average move down for the previous nine daily candles are calculated. These are then compared with the current weekly move up and current weekly move down to find the remaining potential move available for the week.

If either the weekly move up, or weekly move down, have already exceeded the value specified in the parameters, the target required would be a move in the opposing direction, which makes no sense. However, before placing an order, the distance between the target and entry is always tested and no order will be placed if it is less than or equal to zero.

**Target Type Value:**

As described above, the "Target type value" works in conjunction with the selected "Target type". For instance, if "Target type" is TARGET\_FIXED\_PIPS, setting this value to 50 means that the initial target will always be 50 pips from the entry level.

**Reduce target by percentage \(0-100\):**

This parameter is used to reduce the profit target by a set percentage in order to increase the probability that the target will be hit. This is to avoid trying to close an order at the time where there is significant competition with other traders.

**Update target on new opposing zone:**

If this parameter is set to true when the initial target is set to be based on an opposing zone, the EA will update the target for a trade when a fresh opposing zone forms on the same time frame as the zone used to generate the initial target. The new target will be calculated at the new zone entry, but modified by the Target Buffer or Reduce target by percentage

**Close trade when price hits opposing Bollinger Band:**

If set to true, this parameters causes an active buy trade to be closed as soon as the high of the current candle touches the upper Bollinger band. An active sell trade will be closed as soon as the low of the current candle touches the lower Bollinger band. The principle behind this is that the Bollinger band represents a level where price has been over extended away from the moving average due to a strong move away from it. Therefore support or resistance from zones is likely to be move effective and a reversal is more likely. Typically, this would be used when price has been away from an old zone for long time and has only just come back to test it.

**BUFFER VALUES**

**Entry Buffer in pips**

The value in this parameter will move the order entry closer to price to give a higher probability of the order being triggered.

**Stop buffer in pips**

The value in this parameter will move the order stop loss further from price such that the order is not stopped out if price passes though it by just a few pips.

**Target buffer in pips**

As an alternative to the previous parameter, this can be used to reduce the calculated profit target by a set number of pips, instead of a percentage of the total profit target.

**TRADE TARGET FILTERS**

**Minimum target Rs required:**

The value of 1R is always considered as the distance between the order entry and the stop loss. Once an initial target price for a zone has been calculated and set according to the previous setting, it will equate to a given multiple of Rs. In instances where this number of Rs is less than the parameter value, the zone will be considered invalid and no orders or trades will be placed on a retest.

The purpose of this parameter is to ensure that there is sufficient profit margin available relative to the risk associated with the trade.

**Minimum target pips required**

The distance between the order entry and the targe can be specified as a number of pips. Once an initial target price for a zone has been calculated and set according to the previous setting, it will equate to a given multiple of Pips. In instances where this number of Pips is less than the parameter value, the zone will be considered invalid and no orders or trades will be placed on a retest.

The purpose of this parameter is to ensure that there is sufficient profit margin available relative to the risk associated with the trade.

