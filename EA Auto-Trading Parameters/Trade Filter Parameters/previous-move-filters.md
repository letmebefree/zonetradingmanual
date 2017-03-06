# Previous Move Filters

Previous move filters compare previous candle moves with what is happened for the currently forming candle to establish how much of a move might remain during this candle. Any trading can then be restricted if too much of a move in the required direction has already occurred.

The move for each candle is calculated based on whether the closing price of the candle was above \(bullish\) or below \(bearish\) the open price.

For a bullish candle:

·Move up = High – Low

·Move down = Maximum of: High – Close, Open - Low

For a bearish candle:

·Move up = Maximum of: Close – Low, High – Open

·Move down = High - Low

The average move up and average move down for the previous nine candles are calculated. These are then compared with the current candle’s move up and current candle’s move down to find the remaining potential move available for the current candle.

If the zone being retested is supply, the remaining move to occur is considered as the remaining move down available. If the zone being retested is demand, the remaining move to occur is considered the remaining move up available.

If either the current candle move up, or move down, has already exceeded the value specified in the parameters, the potential move remaining becomes 0.

## **Maximum daily move in pips:**

This parameter prevents any orders from being placed in a set direction if a daily move in that direction that is greater that the entered parameter value has already taken place that day.

## **Maximum weekly move in pips:**

This parameter prevents any orders from being placed in a set direction if a daily move in that direction that is greater that the entered parameter value has already taken place that day.

