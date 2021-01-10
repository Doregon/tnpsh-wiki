# Updating the Firmware

1. Remove any disks in the Blu-Ray drive and disconnect the console from the Internet. 
2. Create a folder called "PS3" on the root of your USB storage device. 
3. Create a folder within the PS3 folder called "UPDATE". 
4. Place the desired firmware within the UPDATE folder and rename it "PS3UPDAT.PUP". 
 * If you are on Windows and have file extensions hidden, name it "PS3UPDAT" instead
 * **Rebug releases their firmwares as ZIP files which contain a link to the actual firmware download. A firmware update should have the extension .PUP**
5. Plug your USB storage device into your PS3. 
6. Boot your console into [recovery mode](https://www.reddit.com/r/ps3homebrew/wiki/recovery) by powering it on, holding the power button until it turns off, then holding it again until it does it a quick double-beep. Alternatively, go to the System Update section of Settings.
7. Select "System Update" and choose "Update via Storage Media". It may appear to hang while it checks for an update; so long as the loading icon is spinning, it is searching and it may take hours depending on your storage device.
 * If it reports the data as corrupt, double check the file and folder names, and make sure you chose the correct update for your system (CEX/DEX). 
8. Select the listed update, proceed through the prompts, and allow update to install and reboot.

* You will most likely need to update your apps, such as Multiman or Rebug Toolbox, to fully use them.

* If your USB ports are broken, you can update in Recovery mode by placing the PUP file in `/dev_hdd0/vsh/` on your hard drive or in `/NOT/UPDATE/` on a DVD.

# If you so wish...

## QA Flagging your Console

You can enable the QA flag on your console to allow downgrading from one CFW to a lower version CFW without use of downgrader firmware. It also allows use of the Debug Settings on the XMB.

* For Rebug users: Install Rebug Toolbox, navigate to the far right and select the first option "Toggle QA Flag"

* For non-Rebug users: Install the [Toggle_QA](http://www.mediafire.com/file/ap6rwhm0v2y0ezx/toggle_qa.pkg/file) package and run it. Your console may reboot.

## Update Manager

If you have a QA Flagged console, you can take advantage of the PS3's update manager, and easily switch between firmwares, even if it's a downgrade.

Place pups on your HDD in the following fashion, and they will show up in the System Update menu.
> /dev_hdd0/updater/01/Rebug_4.46.pup

> /dev_hdd0/updater/02/Habib_4.65.pup

> /dev_hdd0/updater/03/Rebug_3.55.pup