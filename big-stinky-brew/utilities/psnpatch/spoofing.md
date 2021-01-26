# IDPS Spoofer Auto-Mode

You can set PSNpatch to automatically spoof an IDPS at boot time.

1. Turn off your console.
2. Press the PS button on your controller to turn the console on.
3. Wait until the PS3 boot up sound is played.
4. Press and hold L3+R3+R2.
5. Wait for 2 beeps and a confirmation message that auto-mode has been set successfully. The system will reboot.

# Spoofing Firmware Version

In the event that a new official firmware is released, you have the option to spoof the firmware to the new version. You can do this by editing the config file found at `/dev_hdd0/game/PSNP11001/USRDIR/PSNpatch.cfg` or `/dev_hdd0/game/BLJS10018/USRDIR/default.cfg` and changing the values for `cobra_spoof_version` and `cobra_spoof_revision` to the latest numbers. These values can be looked up or can be found in an up-to-date SEN Enabler.

The values for 4.84 are:

* cobra_spoof_version=0484

* cobra_spoof_revision=67805

# Changing the CID


You will need a valid CID from another PS3. In the past, PSP CIDs would also work, but this is no longer the case.

1. Use an [FTP program](https://www.reddit.com/r/ps3homebrew/wiki/transferring_files) or multiMAN to browse to /dev_hdd0/game/PSNP11001/USRDIR/ and open PSNpatch.cfg with a text editor. If the folder does not exist, check inside of /dev_hdd0/game/BLJS10018/USRDIR/ for a file called default.cfg.

2. Change the lines "idps=000..." and "psid=000..." to the respective values. If you do not have a matching PSID, leave it as zeroes. It will still work without a matching PSID, but it is potentially slightly more risky. Ensure that both values are 32 digits long.

3. If you used FTP, make sure to upload the file back to the PS3.

4. Launch PSNpatch and press Square to spoof the new CID. Alternatively, if you have set up the PSNpatch plugin, reboot, and press L3+R3+R2 to spoof your CID, disable CFW, and enable PSN access. 

* If you receive error 0x8002A224, this indicates that your CID is not valid.


