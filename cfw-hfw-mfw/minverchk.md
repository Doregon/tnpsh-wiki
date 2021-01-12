# Verifying Compatibility

If your console is one of the 2xxx or 25xx slims, you'll need this too to find out whether or not your console is compatible!

Minimum Version Checker (minverchk) probes your system to find out what the minimum downgrade praxis (discussed on the [About Jailbreaking](../welcome-to-wiki/about-jailbreaking) page) is on your console.

To start, we'll need some things:
* A USB drive
* The minverchk PUP file from the official [PSX-Place post](https://www.psx-place.com/resources/minverchk-minimum-version-checker.610/)
* [7-Zip](https://7-zip.org)
  * macOS users can use p7zip or The Unarchiver. 
  * Linux users can open .7z files natively

1. Download minverchk and save it somewhere you can remember.

2. Install a program that can interact with .7z files and extract the archive.

3. Remove any disks in the Blu-Ray drive and disconnect the console from the Internet. 

4. Create a folder called "PS3" on the root of your USB storage device. 

5. Create a folder within the PS3 folder called "UPDATE". 

6. Place minverchk within the UPDATE folder and rename it "PS3UPDAT.PUP". 
   * If you are on Windows and have file extensions hidden, name it "PS3UPDAT" instead

7. Plug your USB storage device into your PS3. 

8. Go to Settings > System Update and choose to "Update from Storage Media".

minverchk will cause an error but will now display a screen similar to this:

![minverchk]../.gitbook/assets/minverchk_demo.jpg)

**If it shows 3.55 or lower**, you can use a full CFW like [Rebug](rebug/README.md) or [Ferrox](ferrox/README.md).

**If it shows 3.56 or higher**, you can only use [PS3HEN](ps3hen/README.md).