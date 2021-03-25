# External Devices

Have a external drive or a server that you want to dump some backups onto? webMAN supports running games from places other than the internal hard drive. 

# Running Backups over Network

[PS3netsrv](https://www.reddit.com/r/ps3homebrew/wiki/ps3netsrv) is a function that allows you to stream game backups over your network from a PC. You can configure this option in webMAN Games → webMAN Setup → PS3 webMAN [Setup], by entering the IP address of your PS3netsrv server host and the port under the "Scan for LAN games/videos" setting. The games will then show up with the rest of your games in the webMAN games folder on the XMB.

# Running backups on an External Drive

If your game is less than 4GB and your drive is formatted as FAT32, you can get away with using an external hard drive as a backup center, no extra steps required. However, chances are that you’ll be using a NTFS-formatted drive.

Running backups is still easy. Just drop by the [NTFS setup](../../../big-stinky-brew/utilities/ntfs.md) page to get all set up, then use your drive like normal.

# Installing PKGs to an External Drive

webMAN gives you the option to redirect the install location of PKGs to your external hard drive. You can toggle this between a USB device and your internal hard drive by selecting webMAN Games → webMAN Setup → Toggle external gameDATA. After toggling it, you can back out to the XMB and install a package as usual. A folder will be created on your USB device labelled "GAMEI" and will host your installed files. Not all games are compatible with an externalized gameDATA.
