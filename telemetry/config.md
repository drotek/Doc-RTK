#Configuration of the telemetry kit

The Drotek telemetry kit is built to be plug-&-play. It is not necessary to manually configure the kit, as the values and rates are either configured in factory to match the RTK modules settings or automatically configured by Mission Planner or QGroundControl to be used for the RTK application.

However, if you're not using an autopilot system with you RTK setup, manually configuring your telemetry kit can help achieve what you want to do. 

-----

#Manually configuring the telemetry kit for a system with no MAVLink

As said above, using an RTK system without an autopilot (without MAVLink then) implies to configure the telemetry kit according to your RTK setup. 

It is important to note that **all baudrates, for the RTK modules as well as both telemetry boards must be the same**. 

To configure your telemetry boards, you will need to download the _3DR Radio Config_ software. You can download it from [this link](http://vps.oborne.me/). It doesn't require you to install it. When downloaded, extract the archive to a location on your PC of your choice, and then start the software (_3DRRadio.exe_).

<p align="center">
  <img src="./images/3drintro.png?raw=true" alt="3DR Config Main"/>
</p>

This is almost the same as the Mission Planner telemetry setup menu. 












