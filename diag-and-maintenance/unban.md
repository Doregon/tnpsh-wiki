# Unbanning your Console

In the event that your console is banned from PSN, you can unban it by spoofing your Console ID (CID). Your CID consists of two numbers unique to your PS3: The IDPS and the PSID. When your PS3 gets banned, it bans your unique ID from PSN. By spoofing your CID to one of another PS3, you will be able to go on PSN again. You can either buy a private CID from a [trusted vendor](https://www.reddit.com/r/ps3homebrew/comments/2pywcr/ps3_private_consoleid_psid_for_sale_unban_your_ps3/), or use a public CID one found on online. As the names suggest, a with a private CID, you *should* be the only one in possession of it, and it's as if you never got banned in the first place. With a public CID, you will be connecting to PSN along with potentially dozens of other people, and they inevitably get banned quickly.
# Changing the CID

You will need the following:

- [PSNpatch](http://store.brewology.com/ahomebrew.php?brewid=244)

- A valid CID from another PS3.


1. Use an [FTP client](../big-stinky-brew/pc-tools/ftp-client.md) or multiMAN to browse to /dev_hdd0/game/PSNP11001/USRDIR/ and open PSNpatch.cfg with a text editor. If the file does not exist, check inside of /dev_hdd0/game/BLJS10018/USRDIR/.

2. Change the lines "idps=000..." and "psid=000..." to the respective values. If you do not have a matching PSID, leave it as zeroes. It will still work without a matching PSID, but it is potentially slightly more risky. Ensure that both values are 32 digits long.

3. If you used FTP, make sure to upload the file back to the PS3.

4. Launch PSNpatch and press Square to spoof the new CID. Alternatively, if you have set up the [PSNpatch plugin](../big-stinky-brew/utilities/psnpatch/plugin.md), reboot, and press L3+R3+R2 to spoof your CID, disable CFW, and enable PSN access. 

* If you receive error 0x8002A224, this indicates that your CID is not valid. If you receive this error, and are on DEX, see [this page for settings to go online with DEX](../welcome-to-wiki/psn.md).