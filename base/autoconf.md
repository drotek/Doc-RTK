#Autoconfiguration with QGroundControl / Mission Planner

The RTK modules can easily be configured automatically using the QGroundControl or Mission Planner softwares, which will set up your module as you want without having to go deep into the configuration processes for the Ublox chip.

## QGround Control

In order to configure the base, you need: 
* 1 Computer, used as ground control station
* 1 Micro USB cable
* **Latest** version of QGroundControl Software (available [here](https://docs.qgroundcontrol.com/en/getting_started/download_and_install.html))

_Note that PX4 advise to use the MAVLink 2 protocol within your telemetry link in order to use the channel efficiently. It should be the default parameter, but if it isn't, you can follow [these](https://docs.px4.io/en/advanced_features/rtk-gps.html#mavlink2) quick steps._

Begin with plugging your base module through USB to the computer with QGroundControl installed and open. The module should be recognized automatically. Don't forget to place the base module where it has a clear view of the sky, doesn't have too many buildings around, and can hold in place as much as possible.

The software will initiate the **Survey-in** procedure with default parameters. You should see the monitoring box next to the top hotbar, giving details on the **surveying time**, **current accuracy** and **satellites** the base is connected with.

<p align="center">
  <img src="./images/qgsvin.png?raw=true" alt="QG Survey dialog box"/>
</p>

You can set the values for the surveying time and a minimum accuracy in the general settings menu of the QGroundControl software, it's button located on the top left corner of the main window.

<p align="center">
  <img src="./images/qgbutton.png?raw=true" alt="QG General settings button"/>
</p>

<p align="center">
  <img src="./images/qgset.jpg?raw=true" alt="QG RTK settings"/>
</p>

Once the survey-in procedure is complete, the satellites icon in the top hotbar will turn white, and the base module will start sending data to the rover module (if it is set up) through the telemetry link. The RTK will be active and ready to use as soon as the rover module will have been set up!

##Mission Planner

In order to configure the base, you need: 
* 1 Computer, used as ground control station
* 1 Micro USB cable
* **Latest** version of Missiono Planner Software (available [here](http://firmware.ardupilot.org/Tools/MissionPlanner/))

First, connect your base module to the computer with Mission Planner installed. Open the software, and click the _Initial Setup_ button on the top hotbar. In the left panel, click the _Optional Hardware_ section, and open the _RTK/GPS Inject_ menu. 

<p align="center">
  <img src="./images/mp1.jpg?raw=true" alt="MP RTK settings"/>
</p>

You have reached the RTK configuration page. Begin with connecting to your base module, by selecting the COM port corresponding to it, and clicking _Connect_. You won't need to change the baudrate as the connection is using USB protocol, but if necessary, enter 57600.

Once connected, you'll be provided with informations on the behavior of your base module. After checking the _M8P Autoconfig_ box, you will need to use the survey-in method in order to obtain a location for your base. You can set the necessary accuracy and minimum survey-in time in order to get a position for your base. After setting your own parameters, you can click _Restart_ to operate a new survey-in that will store it's obtained position in the list beneath the parameters box.

<p align="center">
  <img src="./images/mp2.jpg?raw=true" alt="MP RTK settings"/>
</p>

Mission Planner allows the user to store and use previous locations for your base setup. You will find all useful informations on [this](http://ardupilot.org/copter/docs/common-here-plus-gps.html?highlight=rtk#base-module-setting-using-mission-planner) page.

From now on, your base is set up, and only requires you to set up your rover module!















