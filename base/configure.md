#Configuration of the Base!

In order to configure the base, you need: 
* 1 Computer
* 1 Micro USB cable
* **Latest** version of UCenter Software (available [here](https://www.u-blox.com/en/product/u-center-windows))
* **Latest** version of Mission Planner Software (available [here](http://ardupilot.org/planner/docs/common-install-mission-planner.html))

###Configuring the Ublox chip

First of all, install the UCenter software on your computer, as well as the Mission Planner software that you will need later on. When done, you can connect your base module to your computer. Open the UCenter software after that, and connect it to your base module using the button in the upper-left corner.

<p align="center">
  <img src="./images/conf/1.png?raw=true" alt="Conf picture"/>
</p>

After connecting, you should be able to enter the Configuration view from the top hotbar.

<p align="center">
  <img src="./images/conf/2.png?raw=true" alt="Conf picture"/>
</p>



In this menu, scroll down on the left panel to find the _MSG (Messages)_ menu. There, open the slide down menu and pick the RTCM1005 messages. After that, check both UART1 and USB checkboxes and click on the _Send_ button.

<p align="center">
  <img src="./images/conf/3.png?raw=true" alt="Conf picture"/>
</p>

<p align="center">
  <img src="./images/conf/22.png?raw=true" alt="Conf picture"/>
</p>

You must repeat these steps for the _RTCM1077_, _RTCM1087_ and _RTCM1127_ messages (respectively GPS, GLONASS and BEIDOU raw data) without omitting to hit the _Send_ button each time, or your changes won't be applied. Checking both UART1 and USB checkboxes will allow the chip to send the messages either from USB or UART1.




















