# General

**Timeframe for placing trades:**

Only zones from the selected time frame will be used for creating new limit orders during auto-testing. If you wish to trade the same strategy for zones on multiple time frames, then multiple instances of the Expert Adviser must be set up on separate charts based on the same symbol.

**Entry Buffer in pips**

The value in this parameter will move the order entry closer to price to give a higher probability of the order being triggered.

**Stop buffer in pips**

The value in this parameter will move the order stop loss further from price such that the order is not stopped out if price passes though it by just a few pips.

**No sell orders above this price**

The value for this parameter can be set so that no sell orders will be placed above the specified price level. This is generally used to prevent further selling from occurring when price has made a significant bullish move, or broken above a key level

**No buy orders below this price**

The value for this parameter can be set so that no buy orders will be placed below the specified price level. This is generally used to prevent further buying from occurring when price has made a significant bearish move, or broken below a key level.

