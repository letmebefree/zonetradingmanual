# Authentication

In order to use the Expert Adviser, each instance must be authenticated against a central registration database. This occurs every time the EA parameters are changed or a new instance of the EA is initiated on a chart. To authenticate itself, an internet connection is required by the Expert Adviser.

The two parameters described below must be populated within the EA parameters to control user authentication. They are typically best stored as a in a baseline Metatrader template so they do not need to be entered each time.

**Username:**

This must be the user name provided when first subscribing to use the Expert Adviser. It will be unique for every person who is using the EA. Ideally, this would be the user name that you have used to register for the forum \(if applicable\), however, this is not mandatory

**License key:**

A license key will be provided when you first subscribe to using the Expert Adviser. This acts as an authentication password that when entered as a parameter with the correct forum username. When the EA initiates itself, it will authenticate these details against the central licensing database as a valid and paid up subscriber for the selected mod of operation. The EA license key is unique to you and should not be shared with any other person.

