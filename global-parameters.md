# CORE PARAMETERS

The following core parameters control user authentication and operating mode of the EA. They are typically best stored as a in a Metatrader template so they do not need to be entered each time.

**Username:**

This must be the user name provided when first subscribing to use the Expert Adviser. It will be unique for every person who is using the EA. Ideally, this would be the user name that you have used to register for the forum \(if applicable\), however, this is not mandatory

**EA License key:**

A license key will be provided when you first subscribe to using the Expert Adviser. This acts as an authentication password that when entered as a parameter with the correct forum username. When the EA initiates itself, it will authenticate these details against the central licensing database as a valid and paid up subscriber for the selected mod of operation. The EA license key is unique to you and should not be shared with any other person.

**Unique EA Identifier:**

This is a numeric value that can be used to uniquely identify each instance of an Expert Adviser running on a given chart. An EA with a unique identifier can only modify orders that were either created by itself, or by another instance of the EA with the same unique identifier.

Running multiple instances of the EA with the same unique identifier allows for strategies that are implemented across multiple currency pairs or for running multiple strategies on a single pair with a shared trade management approach.

**EA Mode of Operation:**

There are four modes of operation available for Zone-Trader Tutor at this stage. These includes:

* EA\_MODE\_FREE 
* EA\_MODE\_LIVE\_ANALYSIS 
* EA\_MODE\_AUTO\_TRADING. 
* EA\_MODE\_BACKTEST \(not currently available to use\)

Each of the modes are summarised below:

**EA\_MODE\_FREE**

This is the default mode when the EA is first loaded. It is used to view zones on the daily, weekly or monthly charts without any trading capability. Setting maximum or minimum time frame to calculate will NOT override the zones calculated.

Whilst operating the EA in this mode, it is possible to filter the zones that appear using any parameters that appear in the sections \*\*\*ZONE\_FILTERS\*\*\*, \*\*\*PRICE CURVE FILTERS\*\*\* and \*\*\*RELATIVE ZONE FILTERS\*\*\*. Values being filtered by the parameters under these sections are those that only change when a new candle opens or when a zone is stopped out. It does not include any parameters filtering values that change every tick \(e.g. values of technical indicators, time of day\). Neither will any trading parameters be relevant in this mode.

**EA\_MODE\_LIVE\_ANALYSIS**

This is a similar mode to EA\_MODE\_FREE, but applies to all time frames, not just daily,  weekly and monthly. The actual time frames used for deriving zones can be controlled by the "Maximum/Minimum time frame to calculate" parameter values.

**EA\_MODE\_AUTO\_TRADING**

This mode must be selected when you want the EA to place a pending \(or market\) order when all criteria for the strategy settings are met. Zones are still displayed on the chart as happens in mode EA\_MODE\_LIVE\_ANALYSIS.

\[**EA\_MODE\_BACKTEST - not currently available\]**

Previous iterations of this EA have presented an option to back-test a strategy prior to running the strategy in Auto-Trading mode. However, this has not yet been implemented in the current version where the focus has been on the auto-trading functionality.

**Maximum time frame to calculate:**

This determines the highest time frame for which zones will be calculated. As a general principle, when zones from a specific time frame are not required for a strategy, it is better not to calculate them at all.

**Minimum time frame to calculate:**

This determines the lowest time frame for which zones will be calculated. It is beneficial to avoid calculating zones for very small time frames \(M15 or less\) as this can degrade the EA performance significantly. Setting of these values should be used in conjunction with “Candles to look back for zones” to optimise performance for the time frame that zones are required. As a general principle, when zones from a given time frame are not required for a strategy, it is better not to calculate them at all.

**Candles to look back for zones \(0=all\):**

This value determines the maximum number of historic candles the EA will look back when identifying and creating zones.

For instance, if the value is set at 2000, but a zone that has not yet been stopped out was first created 3150 candles ago, this zone will neither appear on the chart or be considered by the strategy in any way. A value of about 8000 candles is recommended.

A value of 0 means that all candles available on the broker server will be used. However, this can cause slow performance, especially when identifying zones for smaller time frames.

Place zone entries against candle bodies:

This controls whether the entry level of zones are placed the low/high of a candle wick, or if it is pushed up against the candle bodies to minimise stop size.

