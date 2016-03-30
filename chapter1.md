# Best Practice

ModuOps makes assumptions based on it's roots for how an Operation Session runs. ModuOps takes into account the nuances of Operations Plans for Modular layouts. The original use cases for ModuOps come from Free-mo Operators. Home layouts have also had a hand in steering ModuOps development.

A Free-mo layout has many unique characteristics not found with other Model Railroad setups:
*  Layout is unique at each setup.
*  Layout will never exist in it current iteration again
*  Layout may only exist for 1 day
*  Starting state of the layout is unknown
*  Crew errors occur but these should be self correcting
*  Rolling stock administration is cumbersome and error-prone

ModuOps 1.0 series is based on the original Mad River and Big Timber (MRBT) software. With this in mind and the constraints listed above, this Chapter helps new users understand some of the design decissions of the Application. Most of the Applciation features directly stem from the prior experience with MRBT and New England Free-mo.

## The ModuOps Difference
ModuOps is a random car type generator. The software essentially takes a list of car types and randomly assigns them to locations on the layout. Using car types is the significant difference ModuOps offers.

The strict rules associated with reporting marks add tremendous effort to an Operating Session. The administrative overhead to maintain car reporting marks takes an tremendous amount of time. In fact, the time invested in this task alone typically exceeds the life-span of the layout by many factors.

## Best Practices
ModuOps works best when there is a sourcing yard that sends car types to Consignees. Large layouts can be split into Districts with different yards acting as the source of cars for areas of the Layout. It is even possible to simulate transfers between yards by making the yard itself a Consignee.

ModuOps is Stateless. That means that the system does not store any information about the past, present or future state of the layout. Another advantage in a layout where "Free-running" occurs between formal operations sessions. ModuOps does not need the layout to be setup in any particular manner prior to the operationing session starting.

ModuOps does not have the ability to schedule a "Pick Up". This is the direct result of the software being Stateless.

ModuOps is a modular system allowing for scheduling engine Plugins. The initial release of the software ships with the Free Mad River and Big Timber scheduling engine. The MRBT scheduling engine is a basic random car type generator (each request has a 1/n chance of selection).

Also available is the sMarty scheduling engine. This is also a stateless engine with weighted random selection. The weighted selection is based on the "Cars Per Week" (CPW) number given to the car type. In addition to the weighted selection, the system skews selections to facilitate car blocking.



