### ModuOps 2017.1 Release Notes {#moduops-1-0-0drc3-release-notes}

### Overview

 ModuOps 2017.1 is updated to allow enahnce the operations' realism and begin the process of ModuOps knowning more about the state of a layout during the operations session. New in this version are the addition of car type codes and formal definition of Yards.

#### Scheduling Engines {#scheduling-engines}

##### MRBT {#mrbt}

The MRBT scheduling engine is a replication of the engine provided by the software package called "Mad River and Big Timber" by Lee Salomon. This engine is a stateless, non-biased random car generator based on rollingstock type. Each and every car move is given an equal chance of being selected. Rollingstock location is not tracked by the system \(stateless\). This scheduler does a good job of creating traffic on a layout especially when the number of Consignees is small.

##### sMarty {#smarty}

The sMarty scheduling engine is a stateless, biased psuedo-random car generator based on rollingstock type. Each car move is has a weighting for selection. The weighting does favor selection of rollingstock based on the percentage an individual weight has compared to all other possible movements for a given sample set. Furthermore, once a car type is selected, there is a significant probability the engine will select a matching move for the Consignee selected.

sMarty is intended for layouts operations where a better approximation of Prototypical car rates are desired for an Operating session.

#### New in this Version {#new-in-this-version}

* Expanded Car Type Classifications  

* Added Car Type Code \(Intended to be AAR codes. See Ops Sig [AAR Freight Car Codes](http://www.opsig.org/pdf/AARFreightCarCodes.pdf) and Eric Neubauer's [Guide to Car Types](http://eaneubauer.ipower.com/type.pdf)\)
* Added Modules/Town designation as a Yard
* Added Train origin/destination Yard selection
* Added Yard capacity planning based on Train routes and Consignee requests

#### What's Not Working... {#what-s-not-working-}

Drop Zones in a Module/Town have a "Direction" which is the direction the zone faces to be a trailing drop \(A or B\). Zones that are accessible by both sides of a module are not supporter \(faces A & B\). For now, designate these zones as either an A or B.

### Platform Support

ModuOps supports a variety of platforms.

**Windows  
 **     Windows 7 \(both 32-bit and 64-bit\)  
      Windows 8.x \(Desktop\)  
      Windows 10

**Mac OS  
 **     10.9.x \(Mavericks\) on Intel  
      10.10.x \(Yosemite\) on Intel  
      10.11.x \(El Capitan\) on Intel  
      10.12.x \(Sierra\) on Intel

#### Feedback and Bugs {#feedback-and-bugs}

Your feedback and bug reports are important to us. There's big plans for ModuOps but we can't get there without your help.

Please use our [Forums](http://www.moduops.com/forums) to post Feedback you have on the software.

[Bug reports are tracked on Github](https://github.com/bhall2001/moduops/issues). However, we understand that you may not be familiar with the system so please feel free to post bug reports in our Forums as well.

