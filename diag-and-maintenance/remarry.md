# Remarrying a Blu-Ray Drive

In the event that your Blu-Ray disc drive breaks and you replace it with a new one, you will need to marry it to your console to be able to use it. Keep in mind that you need to have the **same model number of Blu-Ray drive** for it to work. 

1. Remove any discs from inside the drive. 

2. Install [CFW Settings](https://web.archive.org/save/http://www.psxhax.com/threads/cfw-settings-0-1-for-ps3-custom-firmware-by-mysis.127/), or enable if in Rebug Toolbox under the "Selector" column if on Rebug CFW. If you get a black screen while launching Rebug Toolbox, press the eject button on your PS3 or install No-BD firmware.

3. Open Rebug Toolbox, scroll to the far right column, near the bottom and select "Dump eid root key".

4. With a USB storage device plugged in, use an [FTP Program](../big-stinky-brew/pc-tools/ftp-client.md) or multiMAN's file manager to move the eid_root_key from /dev_hdd0/game/RBGTLBOX2/USRDIR/ to /dev_usb00X/ (with X being any number).

5. Turn off your console, swap out old Blu-Ray drive for the new one, and turn it back on.

6. Go back to the XMB and scroll over to the Network column, select Custom Firmware Tools, Service Tools, Advanced Service Tools, then "Toggle Factory Service Mode" to turn FSM on. It may take a few seconds for it to boot into FSM, and a USB cable is required to use your controller.

7. Scroll over to the Network column, select Custom Firmware Tools → Service Tools → Advanced Service Tools → "Remarry Blu-Ray Drive". If successful, a notification should pop up "CEX_drive_init() succeeded".

8. Go back to the XMB and scroll over to the Network column, select Custom Firmware Tools → Service Tools → Advanced Service Tools → "Toggle Factory Service Mode" to turn FSM off.