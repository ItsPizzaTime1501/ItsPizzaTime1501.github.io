# Custom themes guide

Credit to `It'sPizzaTime#4530` on discord for the images and the rest of this terrible guide

## What you need

* A console with Luma3ds installed
* Anemone3ds (note: you should already have anemone if you followed a good guide, if you somehow don't you can get it [here](https://github.com/astronautlevel2/Anemone3DS/releases/latest))

## Finding a theme

1. Open [Themeplaza](https://themeplaza.eu) on your computer
2. Find a theme you like
3. Press on it
4. Use one of the following 2 methods to install the theme

## Method 1: Adding Themes via QR code

1. Hover over the theme's picture with your mouse, a QR code should pop up like this:  
![Theme QR](/files/pic/theme_qr.png)
2. In Anemone, press the right bumper to open the camera
3. Scan the QR code
4. The theme should be added to the list

## Method 2: Adding Themes Manually

1. Press the download button on the theme's page, if you can't locate it here's a picture that should help:  
![Theme Manual Download](/files/pic/theme_manual_download.png)
2. Save the zip somewhere on your pc
3. Insert your 3ds's sd card into your pc
4. Make a `Themes` folder on your sd root if it doesn't already exist
5. Copy the downloaded zip file to the themes folder, if you're having difficulty here's an example:
![Theme Location](/files/pic/theme_location.png)

## Installing the obtained themes

1. Open Anemone on your 3ds if it isn't already open
2. Select the theme out of the list:  
![Theme List](/files/pic/theme_list.png)
3. Hold A + Dpad up and then release A to install the theme
4. Press Start to exit Anemone and return to your home menu
5. Congratulations, you now have a custom theme  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Custom Theme](/files/pic/custom_theme.png)

## Troubleshooting

### Anemone says "Theme extdata does not exist!"

Fix: Set a default theme in the home menu settings

### I get a crash after installing a theme

Fix: Deleting the home menu theme data

#### How to delete Home Menu Theme Data

1. Navigate to the following folder on your SD card:  `/Nintendo 3DS/(32 Character ID)/(32 Character ID)/extdata/00000000/` 

2. Delete the corresponding folder for your region:  
USA: `000002cd`  
EUR: `000002ce`  
JPN: `000002cc`  

#### Anemone Crashes

Fix: Try again, if it still crashes reinstall Anemone, if it **still** crashes delete the `Themes` folder on your sd
