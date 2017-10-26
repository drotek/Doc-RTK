#Frequently Asked Questions

<p align="center">
  <img src="./images/drok.png?raw=true" alt="Drone Drotek"/>
</p>

* **Is it absolutely necessary to have two boards, one rover and one base?**

The RTK technology requires a stationnary receiver to allow exact calculation of the rover module. To achive this, you need **two receivers**, one to act as the base module, and another as the rover module, **whatever the use-case is**. 

-----

* **Do the XL, Tiny and Sirius modules have built-in batteries? Do they need an external power supply?**

The XL RTK module, as well as the Tiny RTK and Sirius RTK modules do **not** have built-in batteries. This means you have to supply power to these boards in order to have them working. You can supply them with power from USB port (excepted for the Sirius RTK module which doesn't have one), for instance with a power bank for smartphones or a computer. The necessary power supply is **5V** so make sure to not oversupply them.

-----

* **Are the Drotek RTK modules compatible with other brands telemetry kits?**

The Drotek RTK modules are compatible with most telemetry kits. In fact, they are compatible with approximately any device that has a serial port using the **UART** protocol. 

-----

* **Can the RTK modules be used without an autopilot?**

The use of an autopilot is not obligatory, even though some of the modules are built specifically for this purpose. Using an autopilot provides a MAVLink in which can be encapsulated the RTK data, and an automatic process that will configure the modules almost entirely automatically. Using the RTK modules without an autopilot will require you to configure the modules in order to be able to communicate with the telemetry boards correctly. You can find more on configuring the RTK modules by following [this link](https://valentinipanini.gitbooks.io/doc-rtk/content/base/configure.html) for the base module, and [this link](https://valentinipanini.gitbooks.io/doc-rtk/content/rover/configure.html) for the rover module.

-----

* **What's the most efficient Survey-in time? How long does it take to reach 1 m. accuracy? 50 cm accuracy? 10 cm accuracy?**

There is no best survey-in time, as it's duration will mainly depend on what accuracy you want to reach. This setting can be set up with either Mission Planner or QGroundControl, as well as the UCenter software in case you don't use an autopilot. Keep in mind that having an efficient survey-in will require to have the base set in the most building-free space and a clear sky-view. The time necessary to reach a 1 meter accuracy for the base positioning is approximately 10 minutes. Reaching 50 cm and below accuracy will require a much longer period of time, roughly an hour, or more. 

In order to get the most accurate position for your base, you can use known reference locations in order to have an accurate position. You should be able to find such places by looking for your national _geodesy_ institute (i.e. it is the [IGN](http://geodesie.ign.fr/index.php?page=points_geodesiques) for France). For the USA for instance, you should find informations following [this link](https://www.ngs.noaa.gov/).

-----

* **Can multiple rover modules be used with a single base module?**

In order to use multiple rover modules with a single base, you have to choose between using a **special telemetry firmware** that will allow multipoint communication (more infformations can be found [here](http://ardupilot.org/copter/docs/common-telemetry-landingpage.html)), or using the TCP/IP protocol to stream the RTK data from the base module. You can find more informations on the configuring of the Ublox chip and its TCP/IP features by following [this link](https://www.u-blox.com/en/product/neo-m8p-series).

-----

* **Is it possible to have multiple bases to increase accuracy?**

It is virtually **impossible** to use multiple base modules for a normal RTK setup, as it would not increase the accuracy, and require a much more complex setup.

-----

* **Are Drotek RTK modules compatible with other brands RTK modules? (i.e. Drotek rover module with other brand base module)**

It is possible to use a Drotek receiver as the rover module, and another brand's RTK receiver as the base module, but this requires to make sure that the data received by the Drotek RTK module contains **RTCM 3** messages.
