# Luma3ds Plugin Loader Guide

This guide will teach you how to install and use 2 custom luma forks with different plugin types

Credit to `It'sPizzaTime#4530` on discord for the images and the rest of this terrible guide

If you're trying to use the ACNL plugin you need to follow the steps in the [ACNL Hacking Discord](https://discord.gg/EZSxqRr)

## Requirements

* A console with boot9strap installed
* A plugin file you want to use (`.3gx` or `.plg`), if you don't have any you can find them by doing a quick google search, here's a list of some good ones:

Pokemon Ultra Sun and Ultra Moon: [ultraSuMoFramework](https://gbatemp.net/threads/release-ultrasumoframework-ntr-plugin-for-ultra-sumo.489098/)

Pokemon Sun and Moon: [sumoCheatMenu](https://github.com/AnalogMan151/sumoCheatMenu/releases)

Mario Kart 7: [Mario Kart 7 Online NTR Plugin](https://github.com/DarkFlare69/MK7-Online-NTR-Plugin-v3/raw/master/MarioKart7.3gx)

The Legend of Zelda: Ocarina of Time 3D: [Zelda-Ocarina-Of-Time-3D-Plugin](https://github.com/Nanquitas/Zelda-Ocarina-Of-Time-3D-Plugin)

Assorted Games: [CTRPF Plugins 3.0](https://www.maxconsole.com/attachments/ctrpf-plugins-master-zip.9248/)

## Installing plugin type `.plg`

1. Download the `boot.firm` from [here](http://badda.de/lumamod/Luma3DS_v9.1-7-gbd15f_mod.7z) and place it on your sd root, make sure you overwrite the current one.
2. Rename your `.plg` file to `plugin.plg`
3. Make a folder called `plugins` if it doesn't already exist in the `luma` folder on your sd
4. Inside of the `plugins` folder make a folder named the titleid of the game you want to use the plugin file for (If you don't know the game titleid you can find a list [here](http://3dsdb.com) or [here](https://hax0kartik.github.io/3dsdb/))
5. Place the `plugin.plg` file in the folder you just created, if you are having trouble understanding here's an example that might help: <br/>
![plg location](/files/pic/plg_location.png)<br/>
(in this example `00040000001B5100` is Pokemon Ultra Moon's titleid)

6. Insert your sd card into your 3ds and boot it up, if you get a luma config screen select `Show NAND or user string in System Settings` and press start
7. Once you're in the home menu, open the rosalina menu (L + Dpad Down + Select by default) and select `Enable Plugin Loader`
8. Press B to exit the rosalina menu<br/>**(note: if the plugin loader is enabled the option will say `Disable Plugin Loader` and if the plugin loader is disabled the option will say `Enable Plugin Loader`)**<br/>
9. When you launch the game you setup a plugin for your screen should flash green during the Nintendo 3ds splash
10. The standard for cheat menus is the select button, if pressing select doesn't work consider reading the readme of the plugin you're using

## Installing plugin type `.3gx`

1. Download the `boot.firm` from [here](https://github.com/mariohackandglitch/Luma3DS/releases/latest/) and place it on your sd root, make sure you overwrite the current one.
2. Make a folder called `plugins` if it doesn't already exist in the `luma` folder on your sd
3. Inside of the `plugins` folder make a folder named the titleid of the game you want to use the plugin file for (If you don't know the game titleid you can find a list [here](http://3dsdb.com) or [here](https://hax0kartik.github.io/3dsdb/))
4. Place your `.3gx` file in the folder you just created, here is an example that could be helpful:
![3gx location](/files/pic/3gx_location.png) <br/> (in this example `0004000000030800` is Mario Kart 7 Rev 01 USA's titleid)
5. Insert your sd into your 3ds and boot it up, if you get a luma config screen select `Show NAND or user string in System Settings` and press start
6. Once you're in the home menu, open the rosalina menu (L + Dpad Down + Select by default) and enable the plugin loader
7. Press B to exit rosalina
8. Open the game you installed a plugin for, your screen should flash green or blue during the Nintendo 3ds splash
9. The standard for cheat menus is the select button, if pressing select doesn't work consider reading the readme of the plugin you're using

## (Optional) How to switch between `3gx` and `plg` loader luma easily

1. Download both `boot.firm`'s ([Luma 3gx Loader](https://github.com/mariohackandglitch/Luma3DS/releases/latest/) | [Luma plg loader](http://badda.de/lumamod/Luma3DS_v9.1-7-gbd15f_mod.7z))
2. Rename both `boot.firm`'s to something else like `Luma3ds_3gx_loader.firm` for the `3gx` loader and `Luma3ds_plg_loader.firm` for the `plg` loader
3. Download and install [PayloadSpinner3ds](https://github.com/SaturnSH2x2/PayloadSpinner3DS/releases/latest) on your 3ds. Here is a QR you can scan with FBI (FBI -> Remote Install -> Scan QR Code)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![PayloadSpinner3ds QR](/files/pic/payload_spinner_3ds_qr.png)
4. Once it's done installing, exit to your home menu and open the app once. It should say `No payloads were found. Refer to README`, just press A to exit
5. Place both firm files in `/3ds/data/PayloadSpinner3DS/payloads` on your sd like this:
![PayloadSpinner3ds payload location](/files/pic/payload_spinner_3ds_payload_location.png)<br/>
  Now when you want to switch between luma plg loader and luma 3gx loader you can open PayloadSpinner3DS and select whichever one you want to use

## Troubleshooting

### **Game crashes when using a plugin**

Fix: Don't use that plugin

### **Screen doesn't flash and plugin doesn't load**

Fix: Check if you got the right titleid, if you're sure you did try a different plugin