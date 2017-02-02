# GLOBAL PARAMETERS

The following parameters are compulsory and are typically stored as a baseline strategy in a Metatrader template so they do not need to be entered each time.

**Username:**

This must be the user name provided when first subscribing to use the Expert Adviser. It will be a unique name for every person who is using the expert advisor. Typcially, this should be the user name that you have used to register for the forum \(if applicable\).

**EA License key:**

A license key will be provided when you first subscribe to using the Expert Adviser. This acts as a password that when entered as a parameter with the correct forum username, authenticating you against the central licensing database as a valid and paid up subscriber. The EA license key is unique to you and must not be shared with any other person.

**Unique EA Identifier:**

This is a numeric value that uniquely identifies the instance of an Expert Adviser running on a given chart. An EA with the given identifier can only delete or modify orders and trades that are created either by the same EA, or by another instance of an EA that is using the same identifier. This allows a global strategy that crosses EA's running on two or more multiple currency pair charts to be used. Each EA could even have different strategy parameter settings.

An important use of this would be the management of risk when running multiple instances of the EA across many different currency pairs.

**Maximum/Minimum time frame to calculate:**

These two parameters determine the highest and lowest time frames respectively for which zones will be calculated. It is useful to avoid calculating zones for very small time frames \(M15 or less\) as this can degrade the EA performance significantly. Setting of these values should be used in conjunction with “Candles to look back for zones” to optimise performance for the time frame that zones are required.

**Candles to look back for zones:**

This value determines the maximum number of historic candles the EA will look back when identifying and creating zones.

 For instance, if the value is set at 2000 but a specific zone that has not yet been stopped out was first created 3150 candles ago, this zone will neither appear on the chart or be considered for opening orders on any retest.

