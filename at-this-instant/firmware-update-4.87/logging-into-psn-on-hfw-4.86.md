---
description: 'The riskier option, typed by u/AzgalorFelore'
---

# Logging into PSN on HFW 4.86

## DISCLAIMER: Do this at your own risk. This can lead to the suspension or a ban of your PSN account.

### Prerequisites:

* USB storage device that is formatted to the [FAT32](https://recoverit.wondershare.com/flashdrive-recovery/format-usb-to-fat32.html) file system.
* Jailbroken PS3 \([HEN](https://www.reddit.com/r/the_new_ps3_homebrew/comments/kbyli9/guide_to_installing_ps3hen_and_some_faq/) in this case\).
* [FileZilla](https://filezilla-project.org/)
* This text file, [ps3-updatelist.txt](http://www.mediafire.com/file/wqcwc341zv2vn3s/ps3-updatelist.txt/file)
* [webMAN MOD](https://store.brewology.com/get/homebrew.php?id=310&fid=2227)
* [multiMAN](https://store.brewology.com/get/homebrew.php?id=24&fid=2200)

### Steps to login to your PSN account without updating to the latest OFW:

[Video showing all the steps ](https://www.youtube.com/watch?v=Z81sFawKmYY)I have typed below.

1. **Install FileZilla** to your computer
2. **Download webMAN MOD and multiMAN on your computer**, connect your pendrive to your computer, then drag and drop the files to your pendrive or any other storage device that is formatted to the FAT32 file system.
3. **Disconnect the pendrive from your computer and connect it to the second USB slot of your console.** After you've connected the pendrive, go to "Package Manager", then "Install package files", and "standard, you'll see both files appear on the menu.
4. **Install webMAN MOD and multiMAN to your PS3**. After you've installed webMAN MOD, you'll have to press x on it so that it activates every time you turn on HEN.
5. Open MultiMAN and go to "system information". **Write down the IP address** that you see on your menu.
6. **Open FileZilla and type your console's IP address** right next to where it says "HOST".
7. After establishing a connection to your console, **drag and drop the "ps3-updatelist.txt" file to the root of the dev\_hdd0** directory shown in FileZilla.
8. **Restart your console, turn on HEN, and try to login to your account.**

