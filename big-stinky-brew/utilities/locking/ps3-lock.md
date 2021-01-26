# PS3 Lock
 
[PS3Lock](http://store.brewology.com/ahomebrew.php?brewid=297) is an authentication-system that allows you to set a personal button combination to protect your PS3 against unauthorized access, or restrict access. You can restrict XMB Settings, deleting of files from the XMB, and system updates. If you are looking for a password-less way to lock the XMB settings, check out [XMB Lock](https://www.reddit.com/r/ps3homebrew/wiki/xmb_lock).

# Installation

1. Install the PS3Lock PKG.

2. Run installer. If you do not use Mamba or PRX Loader, select "Install PS3Lock (dev_hdd0/boot_plugins.txt)", otherwise select a different one using the D-PAD. If you are not sure, select the default option containing "boot_plugins.txt". It will confirm that it has been installed and ask you to restart your PS3.

3. Highlight "Restart PS3" and press Cross.

4. After your PS3 restarts, you will be prompted to create a button combo password. Enter a combo that is at least 2 buttons long, and less than or equal to 10 buttons long. Press R3 to save the combo, or L3 to cancel the combo.

5. Enter the password again to confirm it.

6. Choose the options that you want enabled for your console.
 * PS3 password protection: Prompts for a password on boot up
 * XMB password protection: Prompts for a password every time the XMB is visited
 * PS3Lock settings password protection: Prompts for a password when changing PS3Lock settings
 * USB Authentication: Requires a specific flash drive plugged into the right-most USB port to unlock (see note below)
 * Restricted mode: XMB settings and the ability to delete apps are locked, as well as hiding /dev_hdd0/GAMEZ/.
 * Buzzer - incorrect password: Console beeps when incorrect password is entered
 * Menu sound effects: Enables or disables sound effects on the XMB, as well as trophy sound effects

Note that in order to enable USB authentication, you will need a USB storage device plugged into the right-most USB port containing the "ps3.lock" file on it, and you will need to hover over the USB authentication option and press Square.

7. Press Circle to exit the settings.

* To uninstall, run the installer app and select "Deinstall PS3Lock".

# Opening the Settings

You can re-open the PS3Lock settings menu by pressing R3 + Circle. It will prompt you for the password combo, press R3 after entering it. If it is entered incorrectly three times in a row, it will shut down the PS3.


# Advanced Settings

From inside the PS3Lock settings menu, you can press L1 to view the advanced settings. 

* PS3Lock sleep timer: This can be set to only allow the PS3 to turn off after a specific amount of time. You can change the time in 30 minute increments up to 3 hours.
* Hide "GAMEZ" folder: This will hide or unhide your /dev_hdd0/GAMEZ/ directory.
* Lock XMB settings: This will lock the settings column on the XMB and prompt you for a password. If you press Square, the setting will persist through reboots, but it also requires an account to be set to auto-login or the XMB will not work properly.
* Block system update: If you select your current CFW version, it will block any system updates (automatically done already in Rebug). By pressing Square, the setting will persist through reboots. This option can only be enabled on 4.46+ firmware.
* PS3Lock start delay: This will change the amount of time before PS3Lock becomes active. If an epilepsy warning is shown on bootup, the recommended time is 6-9 seconds, otherwise you may set it to 0-3 seconds. If the menu freezes after first password entry, then try to open the settings menu (R3+O) and increase the delay time and push L2+R2+L3 to restart.
* Language: Allows you to change the language of PS3Lock. You can also edit your own ps3l_lang.db and press Square to import it.
* Set new password: Allows you to change the password combo.

# Miscellaneous Stats

From inside the PS3Lock settings menu, you can press R1 to view some stats that PS3Lock tracks.

# Forgot Password

If you forgot your button combo, you can reset it with one of the following processes.

1. **If you have a USB storage device**:
 - Create and move a file named "ps3lock.reset" to your FAT32 formatted USB device.
 - Plug the USB device into your right-most USB port.
 - Start the PS3 and press R3 + Square + Circle on startup.
 - The ps3lock.reset file will be deleted, and PS3 will prompt you for a new password.

2. **If you are using USB authentication**:
 - Boot into the XMB with the authenticated USB device.
 - Enter a file manager, such as the one included in multiMAN, and delete /dev_hdd0/plugins/PS3Lock/ps3lock_cfg.bin.
 - Reboot your PS3, and it will prompt you for a new password.

3. **If you do not have a USB storage device**:
 - Boot into [recovery mode](https://www.reddit.com/r/ps3homebrew/wiki/recovery).
 - Select Restore File System. The "boot_plugins.txt" will be deleted and all plugins will be disabled.
 - Enter a file manager, such as the one included in multiMAN, and delete /dev_hdd0/plugins/PS3Lock/ps3lock_cfg.bin.
 - Create a new "boot_plugins.txt" and place it on /dev_hdd0/.
 - Reboot your PS3 and it will prompt you for a new password.
