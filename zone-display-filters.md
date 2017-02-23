ZONE DISPLAY FILTERS

The parameters described in this section are used to filter the zones displayed on the chart. By default, active \(unfiltered\) zones will be drawn using thick lines, whilst inactive \(filtered out\) zones will be drawn with thin lines. If it is preferred for inactive zones to be removed completely to give a cleaner looking chart, this can achieved by setting the display parameterd "Invalid zone line width to WIDTH\_0.

ZoneID:

A list of zone identifiers, each one separated by a semi colon ';' can be entered so that only those zones are active on a chart. This can be useful when auto-trading if you only want to target two or three zones to trade retests from. For example, entering the value 'H1\_14864724;H1\_14877936' \(without quotes\) will cause only zones with ID's H1\_14864724 and H1\_14877936 to be displayed as active. This can be seen on the chart below where two zones at the top of the chart are drawn with thick lines.

![](/assets/zonefilter.png)

You will notice that the zone identifier displayed does not include the time frame, but this is required when setting up the parameter.

**Maximum zone depth in pips:**

If the distance between the zone entry and stop level is greater than the parameter value supplied, the zone will be made inactive. It is preferable to trade zones with a smaller distance as these typically provider higher Reward to Risk potential and also allow larger positions sizes and therefore bigger potential profits without increasing overall risk exposure.

**Minimum zone depth in pips:**

If the distance between the zone entry and stop level is less than the parameter value supplied, the zone will be made inactive. If a zone is too narrow, there is unlikely to be any additional orders from smaller time frame zones inside and its strength will therefore be diminished.

