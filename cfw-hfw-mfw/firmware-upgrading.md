# Upgrading Firmware to CFW

Ready to dive into the custom firmware world?

## Upgrading the Firmware

1. Remove any disks in the Blu-Ray drive and disconnect the console from the Internet. 
2. Create a folder called "PS3" on the root of your USB storage device. 
3. Create a folder within the PS3 folder called "UPDATE". 
4. Download your desired CFW of equal or higher version, or a CFW spoofed to the latest version. The most recent firmwares can be found [on this page](https://www.reddit.com/r/ps3homebrew/wiki/firmwares). Regardless of which firmware you choose, [verify the MD5 hash](https://www.reddit.com/r/ps3homebrew/wiki/md5) of the .PUP file to ensure that the file is not corrupt.
   * In order to go to a lower version CFW, you must install a CFW of equal or higher version and then install the [Habib QA Toggle PKG](http://www.mediafire.com/file/kdmyl2g967y15m7/toggleqa.pkg), run it, and reboot before you can install the desired CFW. 
   * If you are on Windows and have file extensions hidden, name it "PS3UPDAT" instead
   * **Rebug releases their firmwares as ZIP files which contain a link to the actual firmware download. A firmware update should have the extension .PUP**
5. Plug your USB storage device into your PS3. 
6. Boot your console into [recovery mode](https://github.com/Doregon/tnpsh-wiki/tree/ec40ea4f7f50454a057c48ec37d7e6bbe67cfd05/cfw-hfw-mfw/recovery.md) by powering it on, holding the power button until it turns off, then holding it again until it does it a quick double-beep. Alternatively, go to the System Update section of Settings.
7. Select "System Update" and choose "Update via Storage Media". It may appear to hang while it checks for an update; so long as the loading icon is spinning, it is searching and it may take hours depending on your storage device.
   * If it reports the data as corrupt, double check the file and folder names, and make sure you chose the correct update for your system \(CEX/DEX\). 
8. Select the listed update, proceed through the prompts, and allow update to install and reboot.
9. You will most likely need to update your apps, such as Rebug Toolbox, to fully use them.
10. If your USB ports are broken, you can update in Recovery mode by placing the PUP file in `/dev_hdd0/vsh/` on your hard drive or in `/NOT/UPDATE/` on a DVD.

## If you so wish...

### Update Manager

If you have a QA Flagged console, you can take advantage of the PS3's update manager, and easily switch between firmwares, even if it's a downgrade.

Place pups on your HDD in the following fashion, and they will show up in the System Update menu.

> /dev\_hdd0/updater/01/Rebug\_4.46.pup
>
> /dev\_hdd0/updater/02/Habib\_4.65.pup
>
> /dev\_hdd0/updater/03/Rebug\_3.55.pup

