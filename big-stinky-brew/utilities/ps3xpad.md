# PS3XPAD

## PS3XPAD

[PS3XPAD](https://mega.nz/#!fNxjBS5Q!z_5zPWrkuJ4UAi8Wy_uNXy9sTjJGOBwO1pV2RWOE7_U) is a plugin that allows you to use non-PS3 controllers on your PS3. The plugin is fully supported in DEX and REX firmwares, check compatibility in the README file for CEX compatibility. [Cobra](https://www.reddit.com/r/ps3homebrew/wiki/cobra) or [MAMBA](https://www.reddit.com/r/ps3homebrew/wiki/mamba) must be installed and enabled.

* If you have issues with PS3 controllers not syncing wirelessly, use your custom controller to hold the button combo Start+Select+R3 to disable PS3XPAD. Alternatively, delete your boot\_plugins.txt \(or mamba\_plugins.txt\) via FTP to return it to working order.
* PS2 and PSP game emulators do not work with PS3XPAD.

## Supported Controllers

While you can use your own custom devices, the following are supported by default as of version 0.8:

* Wired Xbox 360 controller
* Wired Xbox One controller
* Wireless Xbox 360 controller with USB wireless adapter
* Wired DualShock 4
* Wireless DualShock 4 with USB wireless adapter

The following are also supported as of version 0.8 for REX/DEX only, with desired game EBOOTs [converted to debug](https://www.reddit.com/r/ps3homebrew/wiki/eboots):

* Button remapping with DualShock 3 and DualShock 4
* Wireless DualShock 4 without USB wireless adapter
* Rumble and Sixaxis Support for DualShock 4

## Installation

1. Copy the downloaded "plugins" folder to /dev\_hdd0/.
2. Browse to /dev\_hdd0/ and open boot\_plugins.txt in a text editor or create it if it doesn't exist. If you are using MAMBA, the file will be called mamba\_plugins.txt. Do not create the file inside of the plugins folder.
3. Add "/dev\_hdd0/plugins/ps3xpad/xpad\_vsh.sprx" to the file and save.
4. Reboot your console. You may get a confirmation message "XPAD Loaded \(VSH\)", but not necessarily.
   * At this point, PS3XPAD may work with your new controller. If not, start your game and wait until it has fully booted, and then press START+SELECT+R3, you should see a confirmation message displaying "XPAD Loaded \(GAME\)". Your controller may disconnect and reconnect.

### Notes

* If PS3XPAD does not work, you may need to press START+SELECT+R3 when switching between a game and the XMB
* Xbox 360 wireless dongles can support up to 4 wireless controllers
* With Xbox 360 wireless controllers, you may have to re-sync using a button combo \(START+SELECT+D-Pad-DOWN\) if you switch between the XMB and a game.
* To connect a DualShock 4 controller, you must set the internal Bluetooth address of the controller. It only needs to be set once.
* You can manually change the settings of PS3XPAD via changing the xpad\_settings.txt file within the plugin folder.
* It may be desirable, especially with fighting sticks or arcade boards, to change the "RESPONSE\_TIME" option to a lower value. Lower values will decrease input latency, but may affect your FPS for some games. The recommended for a DualShock 4 is at most 7. Generally, there are no issues with setting the value to 5.

## Using a Custom Device

You can use up to 24 custom devices by editing the xpad\_devices.txt file in the plugin folder. Following the template of the other devices in the xpad\_devices.txt file, you will need to find the VID and PID for your device, followed by your name for the device, and its XTYPE. You can just copy the line containing your device's information from [this PS3XPAD devices list](https://pastebin.com/raw/YTMN99eM) to xpad\_devices.txt and save it, or you can create one manually with the process below.

* Entering the incorrect values will result in an error prompting "Unknown USB Device". 

### Creating a Config

To create a config, you will need to find the VID and PID of your device, and also choose the closest XTYPE. **It is advised to use a powerful text editor such as Notepad++ to create these, as some text editors will add invisible characters that will break the config**.

1. To find the VID and PID: On Windows, navigate to Start → Control Panel → Type "Device Manager" in the search bar and select it → Find your device and right click it → Properties → Details tab → Select "Hardware Ids" on the drop down menu. The characters following the underscore after VID or PID are the needed values. Make sure to put "0x" before each value to match the template.
2. For the XTYPE value, choose the closest-matching out of these:
   * XTYPE\_XBOX
   * XTYPE\_XBOX360
   * XTYPE\_XBOX360W \(this is a wireless controller, which uses a wireless dongle\)
   * XTYPE\_XBOXONE
   * XTYPE\_UNKNOWN
   * PTYPE\_PS3
   * PTYPE\_PS4
   * PTYPE\_BT \(this requires a Bluetooth dongle\) 
3. Enter your found values into this format: `VID, PID, NAME, XTYPE`. An example config would be: `0x045e, 0x028e, Microsoft X-Box 360 pad, XTYPE_XBOX360`.
4. Save and re-upload this file to your PS3 and reboot for it to attempt to re-detect your devices.

