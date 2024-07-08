# Fruitbox-Extended
This repository includes pre-made files to help fill in some of the gaps of your Fruitbox V2 installation on Raspberry Pi OS.

Fruitbox.ini - This first file is a pre-made fruitbox.ini file that enables the skin chooser and makes some changes to how Attract Mode is set to make it function as a random autoplay. It also sets music folder locations that are not enabled by default. **To install, from a terminal type (or copy/paste) the command below and press enter. For Bookworm or Bullseye OS.**

```wget -O /home/pi/fruitbox/fruitbox.ini -L https://raw.githubusercontent.com/jaythom1/Fruitbox-Extended/main/fruitbox.ini```


The next file will put a shortcut to Fruitbox on your desktop. **To install, from a terminal type (or copy/paste) the command below and press enter. For Bookworm or Bullseye OS.**

```wget -0 /home/pi/Desktop/fruitbox.sh -L https://raw.githubusercontent.com/jaythom1/Fruitbox-Extended/main/fruitbox.sh```

In order for this shortcut to work, you'll need to right click on it once you see it on the desktop and choose ‘Properties’. In ‘Properties’, ignore ‘General’ tab and go to the ‘Permissions’ tab. In Access Control make these settings as needed. I use these: View Content: Only Owner - Change Content: Only Owner - Execute: Only owner Once those are set, click OK. You should now be able to double click that file and a box will open asking if you want to execute file. Click the execute button. Fruitbox should launch.

To remove the “execute this file” dialog nag, open the file below (you might need to ensure ‘show hidden‘ is enabled as the .config folder is hidden by default)> /home/pi/.config/libfm/libfm.conf Find the line quick_exec=0 and change it to quick_exec=1 Save the file and reboot the pi. Now fruitbox should launch by double clicking that bash file on the desktop without getting the execute file dialog.

If you are using a touchscreen, Open File Manager and go to “Edit>Preferences” Put a check in “Open files with single click”. This will remove the double tap requirement making it easy to launch with a single touch of the icon.


This file below will make your Fruitbox launch when you turn on your Raspberry Pi. Please note this is only for the Bookworm versions of Raspberry Pi OS. **To install, from a terminal type (or copy/paste) the command below and press enter.**

```wget -O /home/pi/.config/wayfire.ini -L https://raw.githubusercontent.com/jaythom1/Fruitbox-Extended/main/wayfire.ini```


This file below will set the Raspberry Pi taskbar to autohide. This is a requirement for Fruitbox to work properly.  Please note this is only for the Bookworm versions of Raspberry Pi OS. **To install, from a terminal type (or copy/paste) the command below and press enter.**

```wget -O /home/pi/.config/wf-panel-pi.ini -L https://raw.githubusercontent.com/jaythom1/Fruitbox-Extended/main/wf-panel-pi.ini```

