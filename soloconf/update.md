# Updating the 3DR Solo firmware

For the 3DR Solo drone to be compatible with RTK messages, you need to install a specific firmware. To download this firmware, you can follow [this link](https://github.com/drotek/ardupilot-solo/releases/download/solo-1.5.3/ArduCopter-v2.px4) to download the Drotek-made firmware to install onto your drone.

![Update screenshot](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/soloconf/images/up1.png?raw=true)

To update the 3DR Solo firmware, you'll need to install the WinSCP software \(you can find it [here](https://winscp.net/eng/docs/lang:en) in order to connect to your Drone using the SCP protocol.

Before starting the software, make sure to turn your drone and its controller on.

![Update screenshot](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/soloconf/images/up2.png?raw=true)

With the software open, to connect to the Solo drone, use these informations:

* Protocole SCP
* Nom d’hôte : 10.1.1.10 \(Solo's IP adress\)
* Nom d’utilisateur : root
* Mot de passe : TjSDBkAu
* Port 22

Then click _Connect_ to start the communication.

You will see a new window, in which the left side represents your local files, and on the right the distant machine \(here, the Solo drone\) and its files.

When connected, all you will need is to copy the fille you've just downloaded from the Drotek Github into the _/firmware/_ folder of the drone.

Once the firmware copied, you'll need to close the connection, and restart the drone. After restarting, the drone will enter _Party mode_, in which all LEDs blink in multiple colors in order to indicate that the update process is going on. Once the update will be done, the Drone should restart automatically.

