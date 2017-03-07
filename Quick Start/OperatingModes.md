# Operating Modes

## **EA Mode of Operation:**

There are three selectable modes of operation for Zone-Trader Tutor available. 

The available modes include:

* EA\_MODE\_FREE\_ANALYSIS 
* EA\_MODE\_LIVE\_ANALYSIS 
* EA\_MODE\_AUTO\_TRADING.

If a mode is selected which is not part of the current subscription, the EA will report an error and remove itself from the chart.

Each of the available modes are summarised below:

**EA\_MODE\_LIVE\_ANALYSIS**

This mode is used to view zones on the chart without any auto-trading. It can be used when all trades and orders are to be placed manually. Whilst operating the EA in this mode, it is possible to filter the zones that appear using any parameters that appear in the"Chart Analysis" parameter section of this document. Values being filtered by the parameters under these sections are typically those that only change when a new candle opens or when a zone is stopped out. It does not include any parameters that  change every tick \(e.g. current values of technical indicators, or the current time of day\). Historic values of technical indicators may be used \(e.g. did any part of a zone extend beyond the outer Bollinger band at the time the zone was first created\)

**EA\_MODE\_FREE\_ANALYSIS**

This is the default mode when the EA is first loaded.  It is essentially the same as the previous mode, but only works for the daily, weekly and monthly time frames.  No auto-trading functionality is available when in this mode.

**EA\_MODE\_AUTO\_TRADING**

This mode must be selected if you want the EA to place pending \(or market\) orders when all criteria for the strategy settings are met. As well as the parameters that control the display of zones in LIVE\_ANALYSIS mode, there are many other parameters available that are specifically associated with tick based values such as the current time of day or the current value of a technical indicator. There are also parameters used to manage setting of targets, stops, when to exit trades, position sizing and overall account exposure.

