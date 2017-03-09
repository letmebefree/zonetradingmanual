# Zone Attribute Filters

### IDs:

A list of zone identifiers, each one separated by a semi colon ';' can be entered so that only those zones are active on a chart. This can be useful when auto-trading if you only want to target two or three zones to trade retests from. For example, entering the value 'H1\_14864724;H1\_14877936' \(without quotes\) will cause only zones with ID's H1\_14864724 and H1\_14877936 to be displayed as active. This can be seen on the chart below where two zones at the top of the chart are drawn with thick lines.

![](/assets/zonefilter.png)

You will notice that the zone identifier displayed does not include the time frame, but this is required when setting up the parameter to avoid any possible ambiguity.

## **Maximum zone depth in pips:**

If the distance between the zone entry and stop level is greater than the parameter value supplied, the zone will be made inactive. It is preferable to trade zones with a smaller distance as these typically provider higher Reward to Risk potential and also allow larger positions sizes and therefore bigger potential profits without increasing overall risk exposure. A very narrow zone \(e.g. a few pips\) can also be unrealistic to trade against considering variations in spread and general noise affecting price.

## **Minimum zone depth in pips:**

If the distance between the zone entry and stop level is less than the parameter value supplied, the zone will be made inactive. If a zone is too narrow, there is unlikely to be any additional orders from smaller time frame zones inside and its strength will therefore be diminished.

## **Maximum prior retests:**

For each possible zone on the chart, the EA counts the number of times that price has left the zone and then come back to retest it. If the count is greater than the value of this parameter, the zone will be made inactive, For example if price has left and then returned to retest a zone twice, setting the value to 1 or lower will cause the zone to be inactive. The principle is that the more times price has retested a zone, the fewer institutional orders will be remaining to absorb the momentum and create a reversal.

## **Maximum penetration percent:**

This parameter sets a maximum zone penetration allowed by price since the zone first formed. The principle behind this is that the further price has penetrated a zone, the closer it is getting to breaking the stop level. In practice, each zone on the chart probably contains one or more zones from lower time frames. Each of these lower time frame zones will present some resistance to price in the form of institutional orders placed by traders. Each time the zone is retested, orders at each level will be filled. Eventually all orders at all levels within the original zone will be filled and the zone will be broken.

## **Maximum candles since formation:**

If the number of candles that have closed since the zone formed is greater than the value specified, the zone will be made inactive. This allows for trading only rapid retests soon after a zone first forms, a useful method for getting into a new trend at the start. For example, when a chart is in an uptrend, you may want to enter on any rapid retracement back to demand that happens within 10 candles of the demand first being created. Setting the value of the parameter to 10 ensures that no orders are entered for this particular zone after 10 candles have completed.

## Exclude zones if price has closed inside them :

This parameter forces the EA to look from when a zone first formed to the current time, to check whether price has ever closed within the zone. If so, the zone will be made inactive. The principle behind this is that if price has managed to  close inside the zone, then the chances of there being any orders left at the entry level are nil. Of course, there may be other levels within the zone, created from a smaller time frame and these may still provide some supply or demand.

The next chart below shows all the unfiltered zones on the GBPAUD H1 chart. Whilst the next one further down demnostrates what happens when this parameter is switched on. As you can see, zones are removed when price has already closed once inside them since they were created.

![](/assets/priceClosedinside.png)

![](/assets/priceclosedinside2.png)

