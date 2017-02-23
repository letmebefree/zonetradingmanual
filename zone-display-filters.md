ZONE DISPLAY FILTERS

The parameters described in this section are used to filter the zones displayed on the chart. By default, active \(unfiltered\) zones will be drawn using thick lines, whilst inactive \(filtered out\) zones will be drawn with thin lines. If it is preferred for inactive zones to be removed completely to give a cleaner looking chart, this can achieved by setting the display parameterd "Invalid zone line width to WIDTH\_0.

ZoneID:

A list of zone identifiers, each one separated by a semi colon ';' can be entered so that only those zones are active on a chart. This can be useful when auto-trading if you only want to target two or three zones to trade retests from. For example, entering the value 'H1\_14864724;H1\_14877936' \(without quotes\) will cause only zones with ID's H1\_14864724 and H1\_14877936 to be displayed as active. This can be seen on the chart below where two zones at the top of the chart are drawn with thick lines.

![](/assets/zonefilter.png)

You will notice that the zone identifier displayed does not include the time frame, but this is required when setting up the parameter.

