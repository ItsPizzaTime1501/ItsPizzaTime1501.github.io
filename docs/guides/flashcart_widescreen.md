# Flashcart Widescreen Guide

This guide will teach you how to setup widescreen with any nds flashcart running the WoodR4 kernel

Credits to `It'sPizzaTime#4530` on discord for this guide

## What you need

* A 3ds with Luma3ds installed and GodMode9 setup
* A DS Flashcart running WoodR4

## Method 1: Patching `TwlBg.cxi` manually

1. Download [this](/files/flashcart_widescreen/section0_dumper.gm9) and put it in `/gm9/scripts` on your 3ds's SD
2. Insert your SD into your 3ds and power it on while holding start
3. In the GodMode9 main menu press the home button and navigate to `Scripts` > `section0_dumper` and run it
4. When it's done running power off your 3ds and insert your sd into your pc
5. Navigate to `/gm9/out` and copy the file `section0.bin` located there to somewhere on your pc
6. Download `mkpatch_b` from [here](https://puu.sh/E43fN/f7f3eb2f61.zip) and put it in the same folder as `section0.bin`
7. Download [this](/files/flashcart_widescreen/wide.bat) and place it in the same folder as the two other files
8. Double Click the `wide.bat` script and let it run
9. It should have generated a file called `TwlBg.cxi`
10. Make a `sysmodules` folder in the `luma` folder on your sd
11. Copy the `TwlBg.cxi` file to the `sysmodules` folder

## Method 2: Using Sono's TWPatch to patch `TwlBg.cxi`

1. Download and install [TWPatch](https://sono.9net.org/hebrew/TWPatch/data/TWPatch.cia/) on your 3ds
2. Launch TWPatch from the home menu, it looks like this:  
![TWPatch Home Menu](/files/pic/TWPatch_Home.png)
3. Leave your cursor on `Nintendo Default` and press Start + X
4. Wait for it to finish compressing
5. Press Select to exit
6. Power off your console

## Enabling and Disabling widescreen

To enable/disable widescreen you need to enable/disable `loading external FIRMs and modules`
To do that, boot into luma config (select on boot) and select `Enable loading external FIRMs and modules`, if it is enabled that means widescreen is enabled and if it's disabled that means widescreen is disabled.

## (Optional) [Advanced] 16:10 Widescreen cheats

1. Download r4cce from [here](http://hp.vector.co.jp/authors/VA013928/bin/r4cce086.zip)
2. Insert your flashcart's sd into your pc
3. Copy the file `usrcheat.dat` located in `/_rpg/cheats` on your flashcart's SD to somewhere on your pc <br/> (if your flashcart is empty download [this](https://mega.nz/#!rpkhRCLB!yQdCQGOMfm3LZaf6DYOho60w5M530CZAKWu6uvQX_Eo) and extract it to your flashcart's sd root)
4. Open r4cce
5. In r4cce press Ctrl + O and select the `usrcheat.dat` file that you copied to your pc
6. Open [this gbatemp post](<https://gbatemp.net/threads/widescreen-cheats-for-ds-games-on-3ds.543212/>) in your web browser to check if your game has a 16:10 code written for it  
(if it doesn't you're stuck with normal streched)
7. In r4cce, find your game in the list, if it isn't there select `Add Game` and then select `Dup?`. It should bring up a file selection, from there select your `nds` rom
8. Right click on the game title and select `Add Code`
9. Name the code `16:10 Widescreen` or something similar
10. Paste the code from the gbatemp thread into r4cce like this:  
![r4cce HG code](/files/pic/r4cce_code.png)
11. Do this with all of the titles you want 16:10 widescreen for
12. Once you're done save the `usrcheat.dat` by pressing Ctrl + S and  copy the file to `/_rpg/cheats` on your flashcart's SD, replace the existing one when prompted to
13. Insert your flashcart's sd into your flashcart
14. Power on your 3ds and launch your flashcart from the home menu
15. Navigate to your nds game and press Y on it
16. Press X to open the cheat menu and select the widescreen code
17. Press X again to save
18. Launch the game and it should be widescreen 16:10
