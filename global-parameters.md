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

d

**Maximum/Minimum time frame to calculate:**

These two parameters determine the highest and lowest time frames respectively for which zones will be calculated. It is beneficial to avoid calculating zones for very small time frames \(M15 or less\) as this can degrade the EA performance significantly. Setting of these values should be used in conjunction with “Candles to look back for zones” to optimise performance for the time frame that zones are required. As a general principle, when zones from a given time frame are not required for a strategy, it is better not to calculate them at all.

**Candles to look back for zones:**

This value determines the maximum number of historic candles the EA will look back when identifying and creating zones.

For instance, if the value is set at 2000, but a zone that has not yet been stopped out was first created 3150 candles ago, this zone will neither appear on the chart or be considered by the strategy in any way. A value of about 8000 candles is recommended.

