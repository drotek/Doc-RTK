#Autoconfiguration with QGroundControl / Mission Planner

The RTK modules can easily be configured automatically using the QGroundControl or Mission Planner softwares, which will set up your module as you want without having to go deep into the configuration processes for the Ublox chip.

The rover module barely needs configuration, as it will mainly receive the differential data, either from the autopilot or directly from a telemetry that's plugged to the module.

If you chose to inject the differential data into the MAVLink between your vehicle and a ground control station (i.e. a computer), you only need to connect your rover module to your autopilot. If you're using a Drotek Pixhawk 3 PRO autopilot, then simply plug it into the GPS port of the autopilot. This will supply power to the module, as well as providing it with differential data from the MAVLink.

If you're not using a Pixhawk 3 PRO autopilot, take care of the pinout of the module you're using. You can find all the pinouts for the Drotek RTK modules on [this](https://valentinipanini.gitbooks.io/doc-rtk/content/rtkmodules/table.html) page.

<p align="center">
  <img src="./images/co.jpg?raw=true" alt="Pixhawk XL Connect"/>
</p>
















