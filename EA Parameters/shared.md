# Shared Parameters

The following core parameters control the operating mode and overall behaviour of the EA. They are typically best stored as an in a Metatrader template so they do not need to be entered each time.

## **EA Identifier:**

This is a numeric value that can be used to uniquely identify each instance of an Expert Adviser running on a given chart. An EA with a unique identifier can only modify orders that were either created by itself, or by another instance of the EA with the same unique identifier.

Running multiple instances of the EA with the same unique identifier allows for strategies that are implemented across multiple currency pairs or for running multiple strategies on a single pair with a shared trade management approach.

## **Mode of Operation:**

There are two modes of operation available for Zone-Trader Tutor at this stage. These includes:

* EA\_MODE\_LIVE\_ANALYSIS 
* EA\_MODE\_AUTO\_TRADING. 

Each of the modes is summarised below:

EA\_MODE\_LIVE\_ANALYSIS

If using the free version of the EA, zones will only be displayed on the daily, weekly and monthly charts. It is then possible to filter the zones using any parameters that appear in the sections \*\*\*ZONE\_FILTERS\*\*\*, \*\*\*PRICE CURVE FILTERS\*\*\* and \*\*\*RELATIVE ZONE FILTERS\*\*\*. Values being filtered by the parameters under these sections are those that only change when a new candle opens or when a zone is stopped out. It does not include any parameters filtering values that change every tick \(e.g. values of technical indicators, time of day\). Neither will any trading parameters be relevant for this mode.

If using the paid for version, the EA will operate in a similar manner, but applies to all time frames, not just daily,  weekly and monthly. The actual time frames used for deriving zones can be controlled by the "Maximum/Minimum time frame to calculate" parameter values.

EA\_MODE\_AUTO\_TRADING

This mode must be selected when you want the EA to place a pending \(or market\) order when all criteria for the strategy settings are met. Zones are still displayed on the chart as happens in mode EA\_MODE\_LIVE\_ANALYSIS.

## **Maximum time frame to calculate:**

This determines the highest time frame for which zones will be calculated. As a general principle, when zones from a specific time frame are not required for a strategy, it is better not to calculate them, therefore helping performance.

## **Minimum time frame to calculate:**

This determines the lowest time frame for which zones will be calculated. It is beneficial to avoid calculating zones for very small time frames \(M15 or less\) as this can degrade the EA performance significantly. The setting of these values should be used in conjunction with “Candles to look back for zones” to optimise performance for the time frame that zones are required. As a general principle, when zones from a given time frame are not required for a strategy, it is better not to calculate them, therefore helping performance.

## **Candles to look back for zones \(0=all\):**

This value determines the maximum number of historic candles the EA will look back when identifying and creating zones.

For instance, if the value is set at 2000, but a zone that has not yet been stopped out was first created 3150 candles ago, this zone will neither appear on the chart or be considered by the strategy in any way. A value of about 8000 candles is recommended.

A value of 0 means that all candles available on the broker server will be used. However, this can cause slow performance, especially when identifying zones for smaller time frames.

Place zone entries against candle bodies:

This controls whether the entry level of zones is placed the low/high of a candle wick, or if it is pushed up against the candle bodies to minimise stop size.

