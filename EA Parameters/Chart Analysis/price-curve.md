# PRICE CURVE

The price curve is defined on a higher time frame and represents a range of prices between the closest higher time frame supply zone above the level of interest and the closest higher time frame demand zone below the level of interest.

For example, if the price curve time frame is defined from the D1 chart ,the closest daily supply and demand zones either side of the entry level will be used to define the price curve.

Lets look at a supply zone on the H1 chart that we are considering trading as it is retested. A D1 chart price curve value of 0, means the entry level for the H1 zone is sitting exactly on the stop level of the closest daily supply zone above price. However, a value of 100 means its entry level is sitting exactly on the stop level of the closest daily demand zone.

The lower the price curve percentage is, the lower the zone is sitting on the higher time frame price curve and the higher the probability a trade will work in our favour. The value is representing how much of a trend has already occurred since the last retracement.

The following chart shows an example where an H4 demand zone has its value on the Daily price curve calculated. If we were to consider an H4 supply zone, the price curve values would be reversed with 0% representing the stop level of the closest daily supply zone above price.

![](/assets/pricecurve1.png)

**Price curve time frame type:**

This parameter sets the time frame from which the price curve is defined. In the illustration above, it would have been set to CHART\_D1, so that the price curve is derived from the daily chart.

**Minimum Rs to opposing zone on price curve:**

Whilst the price curve percent represents where the zone entry sits on the higher time frame, it does not give any indication of absolute profit margin to the next opposing zone. Setting this parameter means that any zones with less than the specified number of R’s until the other end of the price curve are automatically set inactive and not used for trading \(1R represents the distance between the entry and stop levels of the retest zone\).

The parameter can be used to stop retests of zones whose entry level is where a significant move on the higher time frame has already occurred.

**Minimum Pips to opposing zone on price curve:**

Very similar to the previous parameter, setting this means that any zones with less than the specified number of pips until the other end of the price curve are automatically set inactive and not used for trading.

**Maximum percent already moved along price curve:**

This value represents the maximum value of the price curve percent value allowed before a zone is set to inactive. For example, if a zone has its entry level sitting halfway between the closest supply and demand zones on the selected higher time frame chart, its percentage value will be 50%. Therefore, setting a maximum value any less that this will cause the zone to be made inactive.

The following chart shows H4 and D1 zones for GBPAUD on the H4 time frame. We see the extent of the higher time frame \(D1\) price curve, as well as the % value shown above each of two H4 zones.

![](/assets/pricecuve2.png)

If we now set the parameter value to 60, the upper zone becomes inactive \(displayed using thin lines\), as shown in the chart below.

![](/assets/pricecurve3.png)

If the restriction is further tightened by adjusting the parameter down to 50, both zones become inactive as shown below.

![](/assets/pricecurve4.png)

