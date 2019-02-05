# Choosing a base module

![Ico base](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/base/images/icobase.png?raw=true)

Chosing the right base module is the first step in order to build an RTK setup that is truly efficient.

The role of the base is as important as the rover's, as the two modules will communicate informations on their position, and having an **accurate positioning for your base will provide best results** for the computing of the position of the rover module.

Even though the chip featured on all of Drotek's RTK modules is the same, the **XXL RTK** module is **designed specifically** for the base role and can't be beaten in this application.

## _Overview_

### XXL RTK

![XXL Base RTK](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/base/images/xxl3D.png?raw=true)

The key features for the base application of the XXL RTK module are it's [Tallysman TW3740](http://www.tallysman.com/index.php/gnss/products/antennas-gpsbeidougalileoglonass/tw3740-tw3742/) **active** antenna, a pair of **rechargeable batteries** included in the case that allow the module to be autonomous and **independant of external power sources**, and a **screw hole** underneath the case to allow it's user to mount it on a tripod and make sure the module is stable and not moving. It's weight because of the antenna and the batteries would easily prevent you from using it as rover, but as a base, weight means a **more stable** and wind-resistant module.

### Tiny RTK

![Tiny RTK](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/base/images/tiny3D.png?raw=true)

The ability to use any antenna you want with the Tiny RTK module allows the user to **adapt the module to it's use-case** and take care of setting up the antenna and the board separately. Using the right kind of antenna that's necessary to one application will allow the user to adapt the module to **his needs**, and reduce the overall size of the base module as necessary, or pick a large antenna for improved performances \(even though size doesn't always mean performance\).

### XL RTK

![XL RTK](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/base/images/xl3D.png?raw=true)

The built-in passive patch antenna will provide you with a ready to use board, preventing you from having to find and buy an antenna to use with the module.

### Sirius RTK

![Sirius RTK](https://github.com/drotek/doc-rtk/tree/062dfb4b3ecf5849b83896a829bb557ce7362f88/base/images/sirius3D.png?raw=true)

The Sirius RTK module **can not be used as a base module**, as it's single 6 pins JST-GH connector is only meant to be connected to an autopilot, which would be configured with RTK data encapsulated into the MAVLink protocol. It's pinout makes it directly compatible with the Pixhawk 3 PRO autopilot.

