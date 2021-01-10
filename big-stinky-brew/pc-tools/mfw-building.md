# MFW Builder

**WARNING: MFW Builder can be a dangerous tool if you do not know what you are doing. It allows you to modify and install firmware with various patches that may or may not brick your console to the point of needing a hardware flasher to restore it. It is recommended to get a NAND/NOR backup of your console and store it on your PC.**

MFW Builder is a PC tool which allows you to use OFW or CFW to create your own modified firmware (MFW). While you can do many things with this, the most useful modifications to existing CFW are adding "no-BD" capability to a firmware and adding an unofficial language pack to your firmware. **It's not recommended to use any other options in the program unless you know exactly what you are doing.**

# Installation

1. Download [MFW Builder 1.0.0 Build 3.1.5](https://github.com/RedDot-3ND7355/PS3MFW-Builder) and extract it.

2. Run the Updater.exe found in the PS3MFW-Builder-master folder.

3. Update the keys by placing [this keys file](http://www.mediafire.com/file/9zbm31vz17f62l6/keys) in the "\.ps3\data\\" folder, overwriting the old one.


# No-BD / No-BT Patches

You can patch a PUP to allow it to install to your console properly if your Blu-Ray or Bluetooth is broken or missing. 

1. In MFW Builder, load your desired "original firmware" (which can be CFW), and choose a directory to save the "modified firmware"

2. For No-BD Firmwares: 
 * Check the "Patch lv1" box on the left side and select "Configure >>" next to it, and check "Patchlv1 noBD Fix for CFW".
 * Check the box next to "Patch PUP" on the left side and select "Configure >>" next to it. Check the "Remove BdpRevoke" and "Remove BD firmware" boxes to create a No-BD MFW. Note that it is dangerous to install No-BD firmware on a console with a working BD logic board.

3. For No-BT Firmware patches:  
 * Check the box next to "Patch PUP" on the left side and select "Configure >>" next to it. Check "Remove Bluetooth firmware" to create a No-BT MFW. Note that it is dangerous to install No-BD firmware on a console with a working Bluetooth OR WiFi dongle.

3. Finish building your MFW and install the generated PUP as a [normal update](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw).


Using Alternate Languages
---

You can patch your firmware to use a language not built in to the PS3. You will need a custom language pack (.LP) file. Currently the only language packs available are [Hebrew](http://www.mediafire.com/file/jv8vkafmr96k87t/Hebrew.LP) and [Greek](http://www.mediafire.com/file/5ya93a6duvu7wo7/Greek-ErMaK86.LP) (4.80/4.81), though [Arabic](http://www.mediafire.com/file/joz5x9o94k37gd8/Rebug_4.81_Arabic_Translation_Beta_4.pkg/file) is supported by an installable PKG. Keep in mind there are small differences between some firmware versions that may make text or symbols be slightly off from where they should be.

1. In MFW Builder, load your desired "original firmware" (which can be CFW). Check the Language Pack check box, and select "Configure >>". Select Browse, and choose the language pack file (.LP). You may need to change the file type dropdown to "All Files" to get the LP file to show up. Choose a language to replace if desired, and check the "Replace Fonts" option if you have a modified font file.

2. Select the "Customize MFW" option, and click Browse next to "Change default Language Pack" to make it the default language.

3. Finish building your MFW and install the generated PUP as a [normal update](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw).

# Creating an Alternate Language

1. Create a folder on your desktop to use as a working directory. Inside this folder create a folder named "replace".

2. (if using a custom font) Create a folder called "font" inside of the working directory, and place your modified font in it. You can modify the default PS3 font (SCE-PS3-DH-R-CGB.TTF found in /dev_flash/data/font/) with a free font editor. 

3. Extract language XML files from RCO files by using RCOmage or LP_RCO. Place all the extracted language files into the "replace" folder.

4. Open the extracted XML files with a text editor, such as Notepad++, and translate all desired text. Only translate text found between the tags (such as immediately before </Text> on any given line). Keep in mind that PS3-specific symbols (such as the X button) will show up as a box in the text.

5. Using a compression tool, such as 7zip, compress the entire working directory in .TAR format. Rename the resulting file's extension to ".LP". 

6. While building your MFW, check the Language Pack check box, and select "Configure >>". Select Browse, and choose your language pack file (.LP). You may need to change the file type dropdown to "All Files" to get the LP file to show up. Choose a language to replace if desired, and check the "Replace Fonts" option if you have a modified font file.

7. Select the "Customize MFW" option, and click Browse next to "Change default Language Pack" to make it the default language.

8. Finish building your MFW and install the generated PUP as a [normal update](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw).