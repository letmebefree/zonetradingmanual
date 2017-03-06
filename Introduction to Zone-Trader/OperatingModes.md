# Operating Modes

**EA Mode of Operation:**

There are three selectable modes of operation for Zone-Trader Tutor available at this stage. These includes:

* EA\_MODE\_LIVE\_ANALYSIS 
* EA\_MODE\_AUTO\_TRADING. 
* EA\_MODE\_BACKTEST \(not currently available to use\)
* EA\_MODE\_HISTORIC\_ZONES.

Each of the modes are summarised below:

**EA\_MODE\_LIVE\_ANALYSIS**

This is the default mode when the EA is first loaded. It is used to view zones on the chart without any trading or placing of order occuring. Whilst operating the EA in this mode, it is possible to filter the zones that appear using any parameters that appear in the sections \*\*\*ZONE\_FILTERS\*\*\*, \*\*\*PRICE CURVE FILTERS\*\*\* and \*\*\*RELATIVE ZONE FILTERS\*\*\*. Values being filtered by the parameters under these sections are those that only change when a new candle opens or when a zone is stopped out. It does not include any parameters filtering values that change every tick \(e.g. values of technical indicators, time of day\)

**EA\_MODE\_AUTO\_TRADING**

This mode must be selected when you want the EA to place a pending \(or market\) order when all criteria for the strategy settings are met.

**EA\_MODE\_BACKTEST**

Previous iterations of this EA have presented an option to back-test a strategy prior to running the strategy in Auto-Trading mode. However, this has not yet been implemented in the current version where the focus has been on the auto-trading functionality.

**EA\_MODE\_HISTORIC\_ZONES**

When placed in this mode, the EA will just display all historic zones, regardless of whether they have since been stopped out or not. This can prove useful for identifying the zone that triggered a historic trade but is otherwise of limited value.

