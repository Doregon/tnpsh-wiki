# FileZilla

## FileZilla

The [FileZilla](https://filezilla-project.org/) client allows you to transfer files can be transferred to and from your PS3. If you have webMAN enabled, an FTP server will always be running in the background, otherwise you can just open multiMAN and it will be running as long as you are in the app. Ensure that you download the "Client" version of FileZilla, not the "Server" version.

## Starting an FTP Session

1. Make sure you have either an Ethernet or WiFi connection between your PS3 and PC.
2. On your PS3, browse to "Network Settings" and test Internet connection. Make note of your PS3's IP address.
3. Open a [FileZilla](https://filezilla-project.org/) session and enter your PS3's IP into the host field in the top left and press enter.
4. In the right-hand side, you should see a directory listing of the different partitions on the drive and USB devices. 
   * /dev\_hdd0/ is your hard drive's main directory
   * /dev\_usb00\#/ is a USB device
   * /dev\_blind/ or /dev\_rebug/ is your flash - Do not modify files here unless you know what you're doing
5. You can browse your PC on the left-hand side and upload or download files by right clicking them and choosing the relevant option on either session. Choosing "Add to Queue" will save the transfer into a list, and pressing Ctrl+P will start processing the list; this is handy if you are not yet ready to transfer large amounts of files.
6. As an alternative to FileZilla, you can open a Windows Explorer window and type in ftp://your.ps3s.IP.here as the file path. This is only recommended for small files because it seems to have a higher failure rate with large files.

## Troubleshooting

* If you cannot see a file that you just placed on your PS3, try pressing F5 to refresh FileZilla's file list.

