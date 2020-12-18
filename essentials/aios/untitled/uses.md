---
description: What can this homebrew be used for?
---

# Capabilities

## Essentially...

### webMAN MOD is capable of the following tasks:

* Direct integration with the XMB menu
* FTP server with remote control functions \(shutdown/restart\)
* WWW server with remote control functions \(scroll down for the complete list of shortcuts\)
* Support for loading and browsing of \[local\] PS3 games in ISO and folder format, DVD videos in ISO format, Blu-ray movies in ISO format, PS1/PS2/PSP games in ISO format with cover display
* NETISO support for network loading and browsing of PS3 games in ISO and folder format, DVD videos in ISO format, Blu-ray movies in ISO format, PS1 and PSP games
* NTFS support for PS3 and PS1 games in ISO format, Blu-ray movies in ISO format and DVD Video in ISO format
* Dynamic Fan Control and in-game temperature monitoring
* PAD shortcuts \(\*open include/combos.h for a complete list of shortcuts\)
* Keep USB device awake
* Mount last game or AUTOBOOT.ISO to system startup \(or HEN enabling\)
* Easy installer/updater
* VSH Menu integration \(hold SELECT to show the menu\)
* sLaunch GUI integration \(hold START or R2+L2 on XMB to show the GUI\)
* New folder icons \(by Brunolee & Berion\)
* Mount PS2 Classics games on PS2 Classic Launcher \(.BIN.ENC\)
* Automatic CONFIG creation for PS2ISOs using config database from ManaGunZ or standalone
* ROMS support through PKG/ROM Launcher and RetroArch
* Auto-mount any custom folder or ISO. Official only can mount AUTOBOOT.ISO
* Title ID can be displayed on XMB menu
* Covers are shown using the Title ID on the file name of the ISO. Official needs to mount the game to show the covers.
* Option for online covers display.
* Rip a game from disc to hdd0 or copy from hdd0 to usb000 or from usb00x to hdd0.
* FTP server includes new SITE commands to allow copy/paste files locally, unmount game, toggle external gamedata, turn on/off dev\_blind, change file attributes
* Safe upload mode prevents a brick/semi-brick if power fails during ftp uploads to /dev\_blind.
* Increased security: ADMIN mode blocks access to critical functions like /setup.ps3, /delete.ps3; Password for FTP server access; limit remote access to specific IP
* Integrated external gameDATA allows installation of packages & game data on external USB drives
* Web Debugger \(remote peek/poke/find bytes\)
* Support for automatic or manual removal of CFW syscalls and spoof console id \(IDPS/PSID\)
* Translated to 23 languages
* Extended support up to 5 remote network servers
* Several shortcuts to toggle Cobra, swap Rebug files, mount net0/ or net1/, show IDPS/PSID, etc.
* Support for user defined combos \(pad shortcuts\)
* Enable screen capture on CFW that don't has the feature.
* Enable selection of emulator for PS1 and PS2 on B/C consoles
* Various improvements on File Manager \(links to navigate faster, mount ISO, mount net0/ or net1/, preview images, copy/paste/delete files & folders\)
* MIN+ memory profile \(same as MIN but uses 512K and 2.5X more buffer for PS3 games\)
* MAX+ memory profile \(same as MAX 1280K for PS3 games, others buffer is reduced, eg: 2X less buffer for ftp and 4X for DVD etc...\)
* Copy operations use shadow copy on hdd0 for faster copy operations
* Scan for games on the stealth folder "/video"
* Support last\_game.txt / autoboot on nonCobra edition
* "Offline" mode \(blocks some PSN/tracking servers\) and automatic restore when CFW syscalls are removed. Game updates still work in this mode. \(v1.33.03\)
* XMBM+ integration when grouping of XMB content is disabled \(v1.33.03\)
* Extended Content Profile Grouping \(v1.33.07\)
* PS3 Manager API Support \(PS3MAPI\)
* Integrated Mysis video\_rec plugin and get klicensee
* Support for .ntfs\[BDFILE\] \(fake ISO created by IRISMAN\)
* Support to mount NTFS games using raw\_iso.sprx \(rawseciso by Estwald\)
* Support for auto-fix games that require higher FW version \(4.20 and later\)
* Optional Video subfolder to "Bluray™ and DVD" folder \(Display RetroXMB videos, videos on USB devices and Data Disc icon\)
* Coverflow-like webGUI aka "slider" provides a mobile/desktop friendly GUI for game selection.
* Optional sMAN-like graphical interface \(GUI\)
* Extended system information \(Title ID, APP Version, IDPS/PSID, CFW version, last played game\)
* Display of Play time & startup time to SELECT+START and /cpursx.ps3 \(Use SELECT+START+R2 to display Game ID, Title, play time and more in-Game info\)
* Virtual pad allows send button events remotely via [http://pad.aldostools.org](http://pad.aldostools.org/) on web browser or with webPAD software \(Windows only\)
* dev\_bdvd/PS3\_UPDATE now is redirected when the plugin is loaded \(and when a game is mounted\) \[This is intended to prevent an accidental update if a game disc is inserted in the drive\]
* /play.ps3 to launch XMB Functions \(e.g: /play.ps3?col=network&seg=seg\_premo\) &lt;- this will start Remote Play server from XMB.
* Once a game is mounted via html, if you click on the displayed icon the game will be launched on the PS3. This is nice to start the game once it's mounted from your mobile This option uses the new command /play.ps3
* Support for auto-play any supported ISO, game folder or auto-open an URL link
* Support for change BD/DVD region
* NETISO server on PS3 \(ISO only\) lets share games among PS3 consoles in a LAN
* Support for local web chat
* Support edition of small text files \(&lt;2KB\)
* Download files & install PKG remotely or with pad shortcuts
* Support batch script automation at startup \(boot\_init.txt\) or played at any time \(/play.ps3/.bat**\)**

