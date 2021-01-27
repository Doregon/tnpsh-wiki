# Data Transfer Utility Exploit

**Note that this method is obsolete due to PS3HAN, and now PS3HEN.**

The Data Transfer Utility \(DTU\) exploit is a method used to move game backups disc-based PS3 game backups and PSP backups from a CFW console to an OFW console, as well as unlock timed trial demos \("C00 demos"\). This method is a CFW2OFW method, but unlike backup injection, it works on all firmwares.

* **This will format and wipe all data on the OFW console**
* Your CFW and OFW PS3s must be on the same unspoofed firmware version number \(eg. 4.81 OFW and Rebug 4.81.2 CFW\)
* PS3 games must have an update available for them or a demo version in order to be compatible with this exploit.
* A compatibility list for CFW2OFW games can be found [here](http://www.psdevwiki.com/ps3/CFW2OFW_Compatibility_List). All C00 games and PSP games should work without requiring updates.

## Converting PS3 Games

Games must be converted to a format that the OFW console can handle.

* You will need:
  * All game files from disc version of your game \(starts with a "B" as in BLUS12345\)
  * [CFW2OFW Helper](https://github.com/friendlyanon/CFW2OFW-Helper/releases)
  * A CFW console
* Extract the contents of the CFW2OFW Helper "Release.zip" to a folder, and place the PS3\_GAME folder from your game into this folder.
* Launch "CFW2OFW Helper.exe". If your game is compatible, the application will automatically download and apply any updates and convert it into an OFW-compatible format \(it will generate a LIC.DAT if needed, and edit the PARAM.SFO\). The resulting game will be put into a folder of the game's name. Repeat this step for all desired games.
* Move the new game folder\(s\) into /dev\_hdd0/game/ on your CFW console.

## Transferring the Games

1. Boot into [recovery mode](https://www.reddit.com/r/ps3homebrew/wiki/recovery) and run option 4, "Rebuild Database". The game should now appear on the XMB.
2. Plug an Ethernet cable into both your OFW and CFW consoles. On the CFW console, navigate to Settings → System Settings → Data Transfer Utility. Choose the first option "Transfer data from this system to the other PS3 system", then select "OK" and let it sit on the "waiting for transfer" screen.
3. On the OFW console, navigate to Settings → System Settings → Data Transfer Utility, and choose the second option "Transfer data from the other PS3 system to this system.". It will prompt you to format the OFW console, select "yes" twice. **This will wipe everything on your OFW console hard drive**. After it is complete, you should be able to play the transferred game\(s\).

