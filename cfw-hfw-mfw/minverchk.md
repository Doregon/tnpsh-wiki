# minverchk

If your console is one of the 2xxx or 25xx slims, you'll need this too to find out whether or not your console is compatible!

Minimum Version Checker \(minverchk\) probes your system to find out what the minimum downgrade praxis \(discussed on the [About Jailbreaking](https://github.com/Doregon/tnpsh-wiki/tree/447f91fc02f93f3f3e121debcda903d9d9144c24/welcome-to-wiki/about-jailbreaking/README.md) page\) is on your console.

To start, we'll need some things:

* A USB drive
* The minverchk PUP file from the official [PSX-Place post](https://www.psx-place.com/resources/minverchk-minimum-version-checker.610/)
* [7-Zip](https://7-zip.org)
  * macOS users can use p7zip or The Unarchiver. 
  * Linux users can open .7z files natively
* Download minverchk and save it somewhere you can remember.
* Install a program that can interact with .7z files and extract the archive.
* Remove any disks in the Blu-Ray drive and disconnect the console from the Internet.
* Create a folder called "PS3" on the root of your USB storage device.
* Create a folder within the PS3 folder called "UPDATE".
* Place minverchk within the UPDATE folder and rename it "PS3UPDAT.PUP".
  * If you are on Windows and have file extensions hidden, name it "PS3UPDAT" instead
* Plug your USB storage device into your PS3.
* Go to Settings &gt; System Update and choose to "Update from Storage Media".

minverchk will cause an error but will now display a screen similar to this:

!\[minverchk\]../.gitbook/assets/minverchk-demo.jpg\)

**If it shows 3.55 or lower**, you can use a full CFW like [Rebug](rebug/) or [Ferrox](ferrox/).

**If it shows 3.56 or higher**, you can only use [PS3HEN](ps3hen/).

