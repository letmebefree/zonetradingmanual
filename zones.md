# Zones

Pending limit orders from institutions are never found at exactly the same price levels, but instead tend to be found in clusters. These clusters of pending orders can be grouped together to create a zone. Typically, zones tend to occur at historic swing points seen on a chart or at areas where there was previously a pause in a price move. In practice, these are areas where institutional order flow has taken place, but either not all sell orders \(supply\) or not all buy orders \(demand\) have yet been filled.

A supply zone is a group of pending sell limit orders above price that will create resistance when price hits that level. The resistance occurs as these limit orders are filled, rather than forcing buyers to transact at a higher price. In a similar way, demand is just a group of pending buy limit orders below price that will create apparent support when price hits that level.

Zones are represented by two lines on a chart, one \(closest to price\) being the entry level and the other \(furthest from price\) being the stop level. Whilst the entry level is a solid line, the stop level is a dashed line.

&lt;image zone representation&gt;

Once price has passed through a zone, that zone is considered invalid as there can no longer be any pending orders remaining in the zone to be filled. The zone is therefore no longer considered by the EA, will not be displayed on the chart and will not be used by the EA for any calculations or derivations of attribute values.

In contrast, inactive zones have not yet been invalidated \(stopped out\), but have been excluded from consideration for trading purposes due to not meeting criteria for the strategy. However, inactive zones are still by default represented on a chart by thinner lines than those used for active zones \(this may be changed through parameters\)

&lt;image inactive zones&gt;

Its important to remember that invalid zones will never be displayed or used by the EA, but inactive zones will not be considered for possible trades but are still used  for calculations such as distance to next opposing zone and the derivation of a price curve. They may also be displayed on the chart, typically with thinner lines than active zones to differentiate them. It is possible to control the line widths, or prevent zones from being drawn at all using the EA display parameters.

On price charts, zones are colour coded based on the time frame that they are derived from.  Colours used for each time frame are as follows:

* MN1 – Green
* W1 – Blue
* D1 – Red
* H4 – Purple
* H1 – Magenta \(Pink\)
* M30 – Orange
* M15 – Lime \(Light Green\)
* M5 – Aqua \(Light Blue\)
* M1 – Yellow

&lt;image colour coded zones&gt;

