# HDD Upgrades

## Upgrading your Hard Drive

This guide will walk you through upgrading the internal hard drive of your PS3 or setting up an external hard drive. For upgrading your internal hard drive, read over the options below to determine which option best suits you.

## Internal Hard Drive

### Installing a Blank Hard Drive

Installing a new hard drive on CFW is the same as installing a new hard drive on OFW. Turn off your console, remove the hard drive, and insert your new one. If it is a NOR console, your PS3 will prompt you to reinstall the firmware from USB at which point you will follow the [normal CFW installation instructions](../cfw-hfw-mfw/firmware-upgrading.md) to complete it, ensuring that you install _the same_ CFW that you were on before swapping the hard drives.

* Keep in mind that a new internal hard drive must be a 2.5" \(9.5mm thick\) drive that runs at 5400rpm, 7200rpm, or is solid state. The maximum size supported for an internal hard drive is 1.75TB. You may need to try it formatted both as MBR and GPT \(both as FAT32\) in order to be recognized and formatted. There's been a very small amount reports of 2TB hard drives working, and a higher rate of success for formatting 1.5TB+ hard drives on 4.55 firmwares.
* Your PS3 will reserve about 10% of the hard drive space as backup sectors and will be unusable for normal operation, even with CFW. On top of this, the firmware will take up approximately 240MB more if it's a NOR console.
* If your PS3 hangs at 100% at the formatting stage, try updating to a newer OFW/CFW on your old hard drive before trying again. 1.75TB support was not added until later firmwares, and therefore requires you to be on a higher firmware.

### Manually Copying Files

This process is the cleanest and quickest method to upgrade your internal hard drive. Essentially, you will determine what files and folders you'd like to save, and copy only those to your new hard drive.

1. Either plug in a USB storage device that can temporarily hold your files and open [multiMAN's file manager \(mmOS\)](https://github.com/Doregon/tnpsh-wiki/tree/b8909682ceb3d35fa1c9004830731e78ed3e8a30/big-stinky-brew/file-managers/multiman/README.md), or [start an FTP session](../big-stinky-brew/pc-tools/ftp-client.md).
2. Copy over the desired files or folders you'd like to back up. Potential files you'd like to back up would be:
   * **/dev\_hdd0/GAMES/** - Folder format PS3 games.
   * **/dev\_hdd0/PS3ISO/** - ISO format PS3 games.
   * **/dev\_hdd0/PS2ISO/** - ISO format PS2 games.
   * **/dev\_hdd0/PSXISO/** - ISO format PSX games.
   * **/dev\_hdd0/PSPISO/** - ISO format PSP games.
   * **/dev\_hdd0/BDISO/** - ISO format Blu-Ray movies.
   * **/dev\_hdd0/DVDISO/** - ISO format DVD movies.
   * **/dev\_hdd0/game/** - Installed games, apps, and DLC.
   * **/dev\_hdd0/home/** - Each folder inside is a user profile which also contains trophy data, PS3/PSP saves, and PS2 saves made with a placeholder launcher.
   * **/dev\_flash2/etc/xRegistry.sys** - This file contains user profile information and is required if you copied user profiles from /dev\_hdd0/home/. 
   * **/dev\_hdd0/savedata/vmc/** - PS2 saves \(disc launcher\).
3. Turn off your console, remove your old internal hard drive from the PS3, and insert your new hard drive.
4. Start your console. If it is a NOR console, it will prompt you for a firmware update, at which point you will follow [these instructions](../cfw-hfw-mfw/firmware-upgrading.md) to re-install your firmware, using the **same firmware you were previously on** \(i.e. Rebug 4.81.2 or Ferrox 4.70\).
5. Restore the content you backed up to the same file paths.
   * If you had backed up your profile\(s\), after copying everything in, shut down your console, boot into [recovery mode](recovery.md) and run the option to Rebuild Database.

### System Backup Utility

This process will create a system back up file on an external hard drive, which you can restore to a new hard drive. If you have a NOR console \(second generation fat or a slim\), you will also need a second USB storage device to apply a firmware update of your current OFW/CFW.

* You will need:
  * The QA Flag enabled; you can check or change this in last column of Rebug Toolbox on any firmware version.
  * Debug Settings enabled; it will show up as the last section in the Settings column of the XMB. If it is not there, try hovering over Network Settings and holding L1 + L2 + R1 + R2 + L3 + DOWN \(D-Pad\).
  * A USB storage device of equal or greater size than your original hard drive 
  * \(For NOR consoles only\) A second USB storage device at least 256MB in size to reinstall firmware
* This process will not save your trophies, so you will need to manually back them up if you want to preserve them. To do this, use multiMAN's file manager or an [FTP session](../big-stinky-brew/pc-tools/ftp-client.md) to navigate to /dev\_hdd0/home/ and copy all of the folders inside of it to a USB storage device or your PC.
* Plug your FAT32 formatted USB storage device your console.
* On your PS3, navigate to the Settings column and select System Settings → Backup Utility → Backup. After it is done backing up, remove your external storage device and plug it into your PC.
* Turn off your console, remove your old internal hard drive from the PS3, and insert your new hard drive.
* Start your console. If it is a NOR console, it will prompt you for a firmware update, at which point you will follow [these instructions](../cfw-hfw-mfw/firmware-upgrading.md) to re-install your firmware, using the **same firmware you were previously on** \(i.e. Rebug 4.81.2 or Ferrox 4.70\).
* Navigate to the Settings column and down to System Settings → Backup Utility → Restore. Select your backup from your USB storage device and wait for it to complete.
  * If you had backed up your trophies, use multiMAN's file manager or an [FTP session](../big-stinky-brew/pc-tools/ftp-client.md) to navigate to /dev\_hdd0/home/ and copy the folders back in, responding "Yes" when prompted to overwrite. After it is finished, shut down your console, boot into [recovery mode](recovery.md) and run the option to Rebuild Database.

### Cloning your Hard Drive to a Same-Size Hard Drive

If you are on CFW, you have the option to move all of your data to a new hard drive via a USB adapter or caddy. If this process should only be done with a new hard drive of equal size, as it will limit the free space on the new hard drive to whatever the size of the old hard drive is.

* You will need:
  * The QA Flag enabled; you can check or change this in last column of Rebug Toolbox on any firmware version.
  * Debug Settings enabled; it will show up as the last section in the Settings column of the XMB. If it is not there, try hovering over Network Settings and holding L1 + L2 + R1 + R2 + L3 + DOWN \(D-Pad\). If you are on DEX firmware, you will need to go into Rebug Toolbox and change _Debug Menu Type_ to CEX QA.
  * A USB adapter or caddy for your new hard drive for the file transfer
* This process will not save your trophies, so you will need to manually back them up if you want to preserve them. To do this, use multiMAN's file manager or an [FTP session](../big-stinky-brew/pc-tools/ftp-client.md) to navigate to /dev\_hdd0/home/ and copy all of the folders inside of it to a USB storage device or your PC.
* Plug your new hard drive into a USB port on your PS3 and select Settings → Debug Settings → Debug for HDD Exchange Utility. Press X to accept the agreement, and X again to confirm the copy.
* After it is finished copying, press X to shut down the console, and then unplug the power cable. Insert your new HDD into the PS3, and power it on. It will rebuild the database. Press X to restart when prompted.
  * If you had backed up your trophies, use multiMAN's file manager or an [FTP session](../big-stinky-brew/pc-tools/ftp-client.md) to navigate to /dev\_hdd0/home/ and copy the folders back in, responding "Yes" when prompted to overwrite. After it is finished, shut down your console, boot into [recovery mode](recovery.md) and run the option to Rebuild Database.

## External Hard Drives

If you are using a new external drive that is above 2TB, you will have to format it as one of the following:

* **FAT32 \(32KB/64KB\)**: Use a PC to format your drive in FAT32, but select 32KB or 64KB Sector Size and MBR \(not GPT\). If your drive is between 2TB and 4TB, use 32KB. If your drive is between 4TB and 8TB, use 64KB. Windows 10 will not have the option to format &gt;2TB FAT32 drives, so you will need to use GuiFormatter to do it. If GuiFormatter won't work, try using WD Quick Formatter, then GuiFormatter. Keep in mind that moving files larger than 4GB will require [one of these methods](https://github.com/Doregon/tnpsh-wiki/tree/b8909682ceb3d35fa1c9004830731e78ed3e8a30/big-stinky-brew/troubleshooting/4gb-files.md).
* **NTFS**: Hard drives beyond 8TB have to be formatted to NTFS and MBR \(not GPT\). Hard drives formatted as NTFS can only be used as an external hard drive. More information can be found [here](hdd-upgrade.md).

If you have issues with webMAN recognizing your external hard drive, open webMAN settings and set "Wait for any USB device to be ready" and "Wait additionally for each selected USB device to be read" to 5 seconds or more.

