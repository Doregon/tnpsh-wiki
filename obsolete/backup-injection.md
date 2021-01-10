# Backup Injection on 4.70 Firmware

**Note that this method is obsolete due to PS3HAN, and now PS3HEN, and is not supported on firmwares greater than 4.70.** 

This guide allows you to run disc-based PS3 game backups and PSP backups, and to unlock timed trial demos ("C00 demos"). This method is similar to the outdated [PeXploit](), with the main difference being that this method allows disc-based PS3 game backups. The exploit, like PeXploit, only works on firmwares **up to and including OFW 4.70**. If you have a higher firmware, see if the [Data Transfer Utility exploit](dtu.md) is right for you.

**PS3 games must have an update available for them or a demo version in order to be compatible with this exploit.** 

* A compatibility list for CFW2OFW games can be found [here](http://www.psdevwiki.com/ps3/CFW2OFW_Compatibility_List). All C00 games and PSP games should work without requiring updates.

## Converting PS3 Games

* You will need:

 * All game files from disc version of your game (starts with a "B" as in BLUS12345)
 * [CFW2OFW Helper](https://github.com/friendlyanon/CFW2OFW-Helper/releases)

1. Extract the contents of the CFW2OFW Helper "Release.zip" to a folder, and place the PS3_GAME folder from your game into this folder. 

2. Launch "CFW2OFW Helper.exe". If your game is compatible, the application will automatically download and apply any updates and convert it into an OFW-compatible format (it will generate a LIC.DAT if needed, and edit the PARAM.SFO). The resulting game will be put into a folder of the game's name. Repeat this step for all desired games.

3. Move the new game folder(s) into "...\TrueAncestor BACKUP Injector\game". 


## Taking a System Backup

1. Plug your FAT32 formatted USB storage device your console. Note that it must be at least the size of your PS3 hard drive.

2. On your PS3, navigate to the Settings column and select System Settings → Backup Utility → Backup. After it is done backing up, remove your storage device and plug it into your PC.


## Injecting Games

* You will need the [TrueAncestor Backup Retailer](http://www.mediafire.com/file/xmo3lsx6dzde659/TrueAncestor_BACKUP_Retailer_v2.20.zip)

1. Extract the TrueAncestor Backup Retailer to a folder and run retailer.exe inside the TrueAncestor folder; it will generate more folders.

2. Browse to your USB storage device on your PC, and drag the numbered folder inside "X:\PS3\EXPORT\BACKUP\" to "\backup\" inside of the TrueAncestor folder.

3. Move your game folder (BLES/BLUS/BCUS/BCES) to "\game\" inside of the TrueAncestor folder.

4. Run retailer.exe and type "1" for "Select Backup Folder" and press enter. Type the number that appears next to your backup and press enter. 
 * To add a game, type "3" and press enter. Type number corresponding to your game and press enter.
 * To add a PSP or "c00" PKG, type "8" and press enter. Type number corresponding to your PKG and press enter.

5. Type "S" for "Inject to Selected Backup" and press enter to begin the injection. Allow it to finish.

6. Move the backup on to your storage device, and plug the storage device back into your PS3. Navigate to the Settings column and down to System Settings → Backup Utility → Restore. Select your backup from your flash drive and wait for it to complete.