# RTK parameters for 3DRSolo

After installing your board inside your Solo and updating its firmware, you will need to set up the Survey-in values in order to get your Solo RTK GPS board to work efficiently.

To do so, first take your ground control station \(computer or laptop\) with Mission Planner installed. Connect your ground control station to the WiFi network of the Solo transmitter. When done, open the Mission Planner software to connect to your Solo though UDP protocol. You will need to select _UDP_ in the dropdown list in the top right corner of the main window, and enter _14550_ as the connection port. If necessary, select 115200 as the baudrate, and if it does not work, try with 57600. Also, it is often reported that the firewall can prevent the connection from being established. Try disabling it or addind a rule for the Mission Planner software and/or open your 14550 UDP port to try and solve the issue.

![UDP Mission Planner](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/soloconf/images/udp.png?raw=true)

Once connected, you can head into the _Initial Setup_ menu, select _Optional Hardware_ and pick _RTK/GPS Inject_ to enter the RTK setup menu.

Here, you should first connect to your RTK Base module by selecting its COM port and the corresponding baudrate \(usually 57600\).

![RTK Mission Planner](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/soloconf/images/mp1.png?raw=true)

Once connected, you'll be provided with informations on the behavior of your base module. After checking the _M8P Autoconfig_ box, you will need to use the survey-in method in order to obtain a location for your base. You can set the necessary accuracy and minimum survey-in time in order to get a position for your base. After setting your own parameters, you can click _Restart_ to operate a new survey-in that will store it's obtained position in the list beneath the parameters box.

![RTK Mission Planner](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/soloconf/images/mp2.png?raw=true)

Mission Planner allows the user to store and use previous locations for your base setup. You will find all useful informations on [this](http://ardupilot.org/copter/docs/common-here-plus-gps.html?highlight=rtk#base-module-setting-using-mission-planner) page.

