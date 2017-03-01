# DISPLAY PARAMETERS

**Hide chart indicators:**

Setting this parameter to true will mean all EA indicators displayed at the top left of the chart will no longer be displayed. This can be used if the chart is already too cluttered and  you are not using this information for manual chart analysis.

**Label value to show on zones:**

LABEL\_RETESTS

With the default value, each zone line has a label such as D1 or S2. This indicates whether the line is demand \(D\) or supply \(S\) and how many retests of the zone have previously occurred. This label

LABEL\_NONE

No label is displayed on either of the zone lines

**Timeframes for zones to display on chart:**

This parameter controls which of the different time frame zones you will see on each of the different time frame charts \(if the zones have not been calculated for the time frame, they cannot be displayed regardless\).

As a rule, zones are typically only displayed on charts from the same or smaller time frame. For example, a daily zone will only be seen on the daily chart or a smaller time frame. It will not appear on the weekly or monthly chart. There are some exceptions to this rule and these will be highlighted below.

When referring to the CHILD time frame, this means the time frame of the chart that is currently being viewed

DAILY\_ONLY

Only daily zones will be displayed and only on D1 or smaller time frames. The following chart demonstrates this when viewing an H4 chart.

![](/assets/display1.png)

WEEKLY\_ONLY

Only weekly zones will be displayed and only on W1 or smaller time frames

WEEKLY\_WITH\_DAILY

Only weekly and daily zones will be displayed. Daily zones will not appear on W1 or MN1  charts and weekly zones will not appear on MN1 chart

![](/assets/display2.png)

CHILD\_ONLY

Only zones relevant to the chart being displayed will be visible. This provides the least amount of clutter possible during manual trading.

![](/assets/display3.png)

CHILD\_WITH\_DAILY

Only the zones relevant to the time frame of the chart being viewed and the daily time frame will be displayed. Daily zones will not be displayed on the W1 or MN1 charts. This is shown below on an H4 chart.

![](/assets/display4.png)

CHILD\_WITH\_WEEKLY

Only the zones relevant to the time frame of the chart being viewed and the weekly time frame will be displayed. Daily zones will not be displayed on the MN1 charts.

CHILD\_WITH\_WEEKLY\_AND\_DAILY

Only the zones relevant to the time frame of the chart being viewed, the daily time frame and the weekly time frame will be displayed. Daily zones will not be displayed on the W1 or MN1 charts. Weekly zones will not be displayed on the MN1 chart.

CHILD\_WITH\_H1

Only the zones relevant to the time frame of the chart being viewed and the H1 time frame will be displayed. This is mainly useful for when manually trading very smaller time frames such as from M15 or M5 charts.

CHILD\_AND\_ONE\_HIGHER\_TIMEFRAME

Only the zones relevant to the time frame of the chart being viewed and the next higher time frame will be displayed. For example, if viewing the H1 chart, only zones from the H1 and H4 time frames will be displayed. When viewing the MN1 chart, only zones from the monthly time frame will be displayed.

![](/assets/display5.png)

CHILD\_AND\_ALL\_HIGHER\_TIMEFRAMES

The zones relevant to the time frame of the chart being viewed and the next higher time frame will be displayed. For example, if viewing the H1 chart, zones from the H1 and from all the other higher time frames \(H4-&gt;MN1\) will be displayed.  This can be useful to get an overall picture of all significant levels from higher time frames, although it can also make the chart look cluttered.

![](/assets/display6.png)

CHILD\_WITH\_ONE\_SMALLER\_TIMEFRAME

The zones relevant to the time frame of the chart being viewed and one lower time frame will be displayed. For example, if viewing the D1 chart, zones from the H4 chart only will also be displayed.

This can be useful if you are trading a time frame such as the H4 manually, but would like to fine tune your entry using a zone from the next smaller time frame.

![](/assets/display7.png)

**Valid zone line width:**

The value of this parameter determines the width of lines for active zones shown on the chart

**Invalid zone line width:**

The value of this parameter determines the width of lines for zones that are not active. Setting this value to WIDTH\_0 means that inactive zones will not be displayed on the chart. However, it is sometimes useful to at least know of their existence, even if you are not interested in trading retests of them.

