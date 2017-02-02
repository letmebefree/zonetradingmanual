# Bias Filtering Parameters

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



