# Trend Bias Filters

The bias is used to filter out zones which would result in trades going against a dominant trend. Whilst they may not always be useful in ranging conditions, they will be beneficial when trading currencies that are in a clear longer term trend. The time frame and direction may either be set manually or calculated by the EA according to the selected parameter value. Refer to the section on "Trend Definition" to understand exactly how the EA determines trend for each time frame

Up to four different biases can be applied at one time. For example, if the bias for the H1 time frame should be up when the trend on the D1, W1 and MN1 time frames are also up, or down when the trend on the D1, W1 and MN1 time frames are also down, each of three different bias settings can be applied using values of BIAS\_D1\_TREND, BIAS\_W1\_TREND and BIAS\_MN1\_TREND respectively. In this scenario, if any of the trends in these three higher time frames are different from the others, there will be no active zones on the H1 chart.

The possible setting are as follows:

BIAS\_NONE

Across all time frames, no bias will be set and both supply and demand zones will be displayed as active. Typically this would be used in ranging conditions.

BIAS\_UP

Across all time frames, only demand zones will be displayed as active on the chart. This would be useful if there was a clear longer term up trend and one was only wanting to trade in the direction of this trend

BIAS\_DOWN

Across all time frames, only supply zones will be displayed as active on the chart.This would be useful if there was a clear longer term down trend and one was only wanting to trade in the direction of this trend

BIAS\_HTF\_TREND

The bias for each time frame will be set according to the trend on the next higher time frame. For example, if the trend on the D1 chart is up, only demand zones will be active on the H4 chart. Similarly, if the trend on the H1 chart is down, only supply zones will be active on the M30 chart. A bias on the MN1 chart will not be set as there is no available higher time frame. This would typically be used for swing trading. where you wanted the EA to adjust bias once the higher time frame trend changed direction.

BIAS\_HHTF\_TREND

The bias for each time frame will be set according to the trend from two time frames higher. For example, if the trend on the W1 chart is down, then only supply zones will be shown as active on the H4 chart. Similarly, if the trend on the MN1 chart is up, only demand zones will be active on the D1 chart. The bias on the MN1 chart will not be set. This may be used in the same way as BIAS\_HTF\_TREND,  but where the next HTF trend was not considered different enough from the trading time frame. For example, if trading M15 zones, then HTF would default to the M30 time frame, whilst HHTF would default to the H1 time frame

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

