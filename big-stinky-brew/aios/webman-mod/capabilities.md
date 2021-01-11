---
description: What can this homebrew be used for?
---

# Capabilities

## Essentially...

### webMAN MOD combines sMAN, webMAN, and aldostools' own code to create a new and powerful all-in-one.

### General

* Support on all custom firmwares with Cobra feature enabled \(ver 4.46-4.87 CEX, DEX & DECR\)
* Support on REBUG firmware with Cobra feature disabled \(ver 4.84.2-4.86.1 CEX & DEX\)
* Support on REBUG firmware with Mamba loaded via boot\_plugins\_nocobra\_kernel.txt \(ver 4.86.1 CEX & 4.84.2 DEX\)
* Support on PS3HEN on 4.82-4.84 OFW CEX & DEX and 4.84-4.87 HFW
* Support on classic custom firmware with Mamba loaded via IRISMAN \(ver 3.41-4.87 CEX & DEX\)
* Support on classic custom firmware with Mamba/PRXLoader \(ver 3.41-4.87 CEX & DEX\)
* Support on classic custom firmware with PRXLoader \(ver 3.41-4.87 CEX & DEX\)
* All PS3 Models \(including all fat, Slim 20xx, 21xx, 25xx, 3xxx & SuperSlims 4xxx\) are supported via PS3HEN payload
* All PS3 Models capable to downgrade to 3.56 or lower are supported via PS3Xploit Flash Writer \(aka PS3Xploit 2.0\) See [this page](http://www.psdevwiki.com/ps3/SKU_Models) for compatibility with CFW

### sMAN / webMAN vanilla features

* FTP server with remote control functions \(shutdown/restart\)
* WWW server with remote control functions \(shutdown/restart/mount/cpursx/insert/eject/setup\)
* Support for loading and browsing of \[local\] PS3 games in ISO and folder format, DVD videos in ISO format, Blu-ray movies in ISO format, PS1/PS2/PSP games in ISO format with cover display
* NETISO support for network loading and browsing of PS3 games in ISO and folder format, DVD videos in ISO format, Blu-ray movies in ISO format, and PS1 games in ISO format.
* NTFS support for PS3 and PS1 games in ISO format, Blu-ray movies in ISO format and DVD Video in ISO format
* Manual and Dynamic Fan Control and in-game temperature monitoring
* PAD shortcuts \(\*open include/combos.h for a complete list of shortcuts\)
* Keep external USB device alive & Reset USB Bus
* Mount last game or AUTOBOOT.ISO to system startup
* Support direct access to NTFS devices through web & ftp \(1.45 / 1.45.11\)
* XMB integration XMB proxy \(1.46 / 1.46.00\)
* Integrated prepNTFS \(1.47\)

### webMAN MOD additional & extended features

**Installer & GUIs**

* Easy installer/updater with 4 editions: full, lite, standard \(rebug\) & nonCobra.
* New icons created by Brunolee & Berion
* VSH Menu integration \(hold SELECT to show the menu\)
* sLaunch GUI integration \(hold START or R2+L2 on XMB to show the game menu GUI\)
* Coverflow web-GUI \(/games.ps3\) provides a mobile/desktop friendly GUI for fast selection of games.
* Grid web-GUI \(/index.ps3\) display games with resizable icons and content can be filtered by type/device/name
* web-GUI for Temperature monitoring: /cpursx.ps3, /cpursx.html & /tempc.html or /tempf.html \(gauges\)
* 2 GUI Themes: sMAN-like graphical interface & webMAN original theme
* LaunchPad integration \(DeViL303' mod to use What's New section to mount games\)
* PhotoGUI integration \(DeViL303' mod to use Photo albums to mount games\)
* XMBM+ integration when grouping of XMB content is disabled \(v1.33.03\)
* Support for custom XML menu \(wm\_custom.xml\) integrated into webMAN Games menu
* Install packages from any folder using web command: /install.ps3

**Localization & Regional settings**

* Translated into 23 languages
* Support for change BD/DVD region

**Content organization & information display**

* Title ID can be displayed on XMB menu \(next to the title or as "info" text\)
* Covers are shown using the Title ID found in the file name of the ISO or folder name \(JB game\).
* Option for display original file name or title name from PARAM.SFO
* Option for display covers as discs, ICON0.PNG or covers from multiMAN, IRISMAN, ManaGunZ repository or in the same folder of the ISO
* Option for online covers display \(free service provided by DeViL303\)
* Optional Video subfolder to "Bluray™ and DVD" folder \(Display RetroXMB videos, videos on USB devices and Data Disc icon\)
* Extended system information via /cpursx.ps3 \(Title ID, game icon, APP Version, IDPS/PSID, CFW version, last played game, console's run time & number of boots\)
* Display of Play time & startup time to SELECT+START and /cpursx.ps3 \(Use SELECT+START+R2 to display Game ID, Title, play time and more in-Game info\)
* Use "home" path to define default path for /app\_home/PS3\_GAME on start up and for R2+START \(e.g. make app\_home start multiMAN or IRISMAN\)
* Support for list NPDRM games stored /dev\_hdd0/game or GAMEI folder on USB FAT32 & NET host, in addition to ISOs and JB folders
* Support for exclude games by file name & Title ID using wm\_ignore.txt

**Extended mount of game**

* Support for multiCD PSXISO games stored as ISO in HDD0 / USB FAT32. Eject/Insert a USB0 device to mount the next CD
* It can mount PSP games stored on exFAT/ext/NTFS/NET devices without copy the file to the internal HDD \(1.47.27\) - Requires prepISO 1.27 or later
* It can mount PS2 Classics games on PS2 Classic Launcher \(.BIN.ENC\)
* Automatic CONFIG creation for PS2ISOs and PS2 Classic using config database from ManaGunZ or the database of CONFIG created by the installer
* Scanning & launch of package files extracted to GAMEI folder on USB FAT32 & NET host. Folders' name can be title\_id or content\_id
* Support for launch SELF applications via PKG/ROM Launcher or through the XMB icon: ★ app\_home/PS3\_GAME
* Integrated external gameDATA allows installation of packages & game data on external USB drives
* Integrated prepNTFS allows to scan PS3ISO, PSXISO, BDISO & DVDISO on NTFS devices without need to run prepISO/prepNTFS
* Support for _.ntfs\[BDFILE\]_ \(fake ISO created by IRISMAN or prepISO/prepNTFS\) - Used to play AVI/MP4 movies or install large packages stored on NTFS
* Support to mount NTFS games using raw\_iso.sprx \(rawseciso by Estwald\) - Supports fake ISO
* Support last\_game.txt / autoboot on nonCobra edition
* Auto install PKG mounted from exFAT/ext/NTFS \(reduce steps needed to install a PKG\)

**Emulation features**

* ROMS support through PKG/ROM Launcher and RetroArch \(support internal HDD/USB/NET storage with custom icons & background images\)
* Enable selection of emulator for PS1 and PS2 on B/C consoles
* PS2 Launcher / PSP Launchers can be integrated into webMAN Games menu for easy access
* Auto install / auto select PSP emulator for PSP games using decrypted MINIS.EDAT / MINIS2.EDAT

**File management & navigation**

* Improvements on File Manager \(file & folder icons, links to navigate faster, mount ISO, mount net0/ or net1/, preview images, copy/paste/delete files & folders\)
* Copy operations use shadow copy on hdd0 for faster copy operations
* It can rip a game from disc to hdd0 or copy from hdd0 to usb000 or from usb00x to hdd0.
* Shorter URL to access paths & files. Use "home" path in /setup.ps3 for search in a user defined folder.
* Support for MD5 hash verification of files stored on PS3 \(internal HDD & USB FAT32 only\)
* Support edition of small text files \(up to 1,300 bytes\) via web
* Hex File Viewer \(internal HDD/FAT32/NTFS/exFAT/ext2\)

**Network features**

* Update to latest release from XMB
* PS3 Manager API Support \(PS3MAPI\) compatible with RTM tools
* FTP server includes new SITE commands to allow copy/paste files locally, unmount game, toggle external gamedata, turn on/off dev\_blind, change file attributes
* Extended support up to 5 remote network servers
* Auto configure remote IP address when /setup.ps3 is accessed from a remote client
* Support navigation of remote network servers even if they are disabled for content scanning
* NETISO server on PS3 \(ISO only\) lets share local games among PS3 consoles in a LAN
* Download files & install PKG remotely or with pad shortcuts
* /dev\_blind and /dev\_hdd1 are auto-mounted when accessed via FTP or http or from XMB
* Support for local web chat \(source code only\)

**Automatization**

* Support for user defined combos \(pad shortcuts\)
* Virtual pad allows send button events remotely via [http://pad.aldostools.org](http://pad.aldostools.org/) on web browser or with webPAD software \(Windows only\)
* Several shortcuts to toggle Cobra, swap Rebug files, mount net0/ or net1/, show IDPS/PSID, etc.
* Automatic remap to /dev\_hdd0/packages on unmount \(SELECT+O\) allows to use Install All Packages on pkg files stored on HDD0
* Support for auto-play on startup any supported ISO, game folder or auto-open an URL link. webMAN vanilla only can mount AUTOBOOT.ISO
* Support for auto-fix games that require higher FW version \(4.20 and later\)
* Support batch script automation at startup \(dev\_hdd0/boot\_init.txt or dev\_hdd0/autoexec.bat\) or played at any time \(/play.ps3/.bat\)
* Launch mounted games with /play.ps3 command. Once a game is mounted via html, click on the displayed icon to launch the game on the PS3.
* Execute XMB functions with /play.ps3 command. \(e.g: /play.ps3?col=network&seg=seg\_premo\) &lt;- this will start Remote Play server from XMB.
* A comprehensive set of web commands and features for customization \(link in Web Commands Documentation\)

**Stealth features**

* Support for dumping IDPS/PSID
* Support for automatic or manual removal of CFW syscalls and spoof console id \(IDPS/PSID\)
* "Offline" mode \(blocks some PSN/tracking servers\) and automatic restore when CFW syscalls are removed. Game updates still work in this mode. \(v1.33.03\)
* Scan for games on the stealth folder "/video"
* Auto unlock savedata during download & copy operations \(removes account id, PSID & copy protection

**Safety & security features**

* Improved temperature monitoring \(max & min fan speed, auto\#2 mode, improved algorithm for dynamic fan control\)
* Increased security: ADMIN mode blocks access to critical functions like /setup.ps3, /delete.ps3; Password for FTP server access; limit remote access to specific IP
* dev\_bdvd/PS3\_UPDATE is redirected to prevent an accidental update if a game disc is inserted in the drive
* Extended Content Profile Grouping \(v1.33.07\) - common files + individual content \(4 profiles\)
* Safe upload mode prevents a brick/semi-brick if power fails during ftp uploads to /dev\_blind.
* System update redirected to /dev\_hdd0/ps3-updatelist.txt using internal proxy \(allows to bypass FW version check on PSN login\)

**Memory & debugging**

* All LV2 peek/pokes are done through syscalls 8/9 \(CFW only\) - syscalls 6/7 used only by PS3HEN
* Web Debugger \(remote peek/poke/find bytes, dump lv1 & lv2 memory\)
* MIN+ memory profile \(same as MIN but uses 512K and 2.5X more buffer for PS3 games\)
* MAX+ memory profile \(same as MAX 1280K for PS3 games, others buffer is reduced, eg: 2X less buffer for ftp and 4X for DVD etc...\)
* Support for up to 3MB from 4 available VSH memory containers \[MC\] \(bg, fg, debug, app\)
* Remote syscalls

**Screen & video capture**

* Capture XMB screen in BMP format
* XMB screen control using /xmb.html \(experimental feature\)
* Enable in-game screen capture on CFW that don't has the feature.
* Integrated Mysis video\_rec plugin and get klicensee used by NPDRM content

