# NTFS
New Technology File System (NTFS) is a file system format for Windows. [Multiman](https://www.reddit.com/r/ps3homebrew/wiki/multiman), [Webman](https://www.reddit.com/r/ps3homebrew/wiki/webman), and [Irisman](https://www.reddit.com/r/ps3homebrew/wiki/irisman) can use NTFS instead of the default format (FAT32) to overcome the limitation of files having to be less than 4GB to transfer them normally. By default, NTFS hard drives work in Irisman, Movian, and Webman 1.45.xx or later. Currently, PS2 ISOs will be temporarily copied to your internal HDD when you mount one, so ensure there is enough space for it to do so.

* Note that your games must be in the same layout as your hard drive: /PSXISO/, /PS2ISO/, /PS3ISO/, /PSPISO/, /BDISO/, and /DVDISO/. 

# prepNTFS for Multiman and Webman

If you are wanting to use a NTFS drive in Multiman, or with Webman (before version 1.45n, such as the one included in Rebug 4.81.2), you will need to use PrepNTFS. Download and install prepNTFS which is found on the [download page of WebMAN](https://github.com/aldostools/webMAN-MOD/releases/). It is recommended to use the newest version from the GitHub, which is made by AldosTools, instead of the outdated official version on Brewology. After running it, you will be able to see your games in the Webman Games folder or in the Retro column of Multiman. Remember that you must have your files are in the correct folders (e.g. PS3ISO, PSXISO).

* **Note that you will need to run prepNTFS every time you add or remove a game from your NTFS device**


# USB Config

In some cases, PrepNTFS won't work to get the drive viewable in Multiman, so you will need to create a text file named "USB.CFG". Inside the file you need to write: `0xaaaa:0xbbbb:#' where "aaaa" is your device's VID, "bbbb" is your device's PID, and "#" being the number of partitions the drive has (default is 1). 

* Example USB.CFG: 0x152d:0x2339:1

Save this file and place it in Multiman's USRDIR folder (/dev_hdd0/game/BLES80608/USRDIR/). Launch Multiman (you will need to select Multiman mode if it shows up as mmCM) and then choose the "Enable PFS Driver". It should now show up as pvd_usb000 in mmOS.

* To find your VID and PID, plug the drive into your PC, browse to Device Manager, find your device under "Disk Drives", right click it and select Properties → Details, then select "Parent" from the drop-down. Displayed will be VEN_aaaa, and DEV_bbbb.