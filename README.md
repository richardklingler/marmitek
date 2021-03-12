## Marmitek Smart Home Devices Reverse Engineering

![Marmitek Power LI](images/powerli.jpg)

This repository contains documentation about Marmitek WiFi Plug Power SE and WiFi socker strip Power Li.
The motivation is to replace the existing WiFi module/firmware with the excellent ESPHome project.

### Sponsoring

All my reverse engineering work is paid with my low little budget, so every donation is very welcome, either through the Patreon link on the side or through Paypal Me:

[Paypal Me](https://paypal.me/renderingfun)

### Update

#### 12.03.2021

- Added first draft of Power Li socket strip schematic
- Added first version of Power Li YAML file

#### 11.03.2021

- Added BL0937 AC measurement IC datasheet used in Power Li strip
- Added TyWE2S and WR3E datasheets
- Added ESPHome yaml file for the Power SE WiFi Plug.
- Uploaded picture of Power SE ESP12-E modification

### Power SE ESPHome modification

Replaced the TYWE2S module with an ESP12-E.

![Marmitek Power SE ESPHome](images/powerse_mod.jpg)

### Power Li ESPHome modification

Replaced the WR3E module with an ESP12-E.

#### What is working

- Switching on/off all 4 relays

#### What is not working

- Although the ESP12E module is pin compatible with the original module, TXD as GPIO1 can't be used for turning on the USB charger supply as during power up TXD detects a pull down and disables booting.

![Marmitek Power Li ESPHome](images/powerli_mod.jpg)

