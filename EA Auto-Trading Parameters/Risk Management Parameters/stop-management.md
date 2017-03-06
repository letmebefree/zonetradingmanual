# Stop Management

## **No hard stop \(fixed lot size used\):**

Prevents any stop being automatically set for orders by the EA. When this value is set, position size cannot be derived according to the trade risk \(now infinite\). Therefore, a fixed lot size is always used, the value of which is taken from the Position sizing parameters.

## **Use trailing stops based on zones:**

Setting this value to true means an active trade’s stop loss is moved each time a new zone forms behind the price move. The time frame monitored for new zones is set in a subsequent parameter. Consider a long trade created after the retest of an H1 demand zone. If the trailing stop time frame is set to H1, as price moves into profit, the stop loss is moved up each time a new demand zone forms behind current price. The stop loss of the trade is adjusted to the stop level of the newly formed zone. Clearly, the new level must be further in profit that the original stop loss. In addition, the EA will only move the stop when the new stop level is better than the breakeven point for the trade.

## **Trailing stop time frame:**

This is used in conjunction with the parameter “Use trailing stops based on zones”.

## **Move to break even at specified Rs:**

When set to a value greater than zero, the EA will move the trade stop loss to the original trade entry level once price has moved into the required number of R’s profit, where R equals the distance between the entry level and stop loss at the time the trade is first activated.

## **Move to break even after specified pips move:**

This works in the same way as the previous parameter, except the minimum profit required before moving the stop loss to breakeven point is specified in pips, not R’s.

