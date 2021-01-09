# OtherOS++

**WARNING: The tutorials on this page involve modifying files in the flash. There is a potential for something to go wrong and being unable to start up your PS3 properly. In this case, it is recommended to have a backup of your flash before proceeding. A brick may or may not be fixable by reinstalling your CFW.**

OtherOS++ is the rebirth of OtherOS, the feature in which you could run Linux on PS3 which was later removed by Sony in official firmware 3.21. OtherOS works on fat PS3 models, as well as slim models which was never possible on official firmware. You can find a list of distributions that worked on OtherOS on [this page](http://www.psdevwiki.com/ps3/Distributions) ([archive](http://web.archive.org/web/20161130030034/http://www.psdevwiki.com/ps3/Distributions)).

A video demonstration of installing Linux can be found on [Modded Warfare's channel](https://youtu.be/yaXOE1sUYAE?list=PLn7ji3VsPy3HtSY6rB8yCCRQpWQOc-uJS).


# Installing Linux

This tutorial assumes you are on Rebug CFW. You will need a keyboard/mouse to navigate Linux, and an empty USB storage device. A CD/DVD will also work.


1. Download the Petitboot image corresponding to your model's flash chip ([NAND](http://www.mediafire.com/file/b8kti561d3o3yso/Petitboot_Minimal_%28NAND%29.zip) or [NOR](http://www.mediafire.com/file/87c7m24lelzypg8/Petitboot_FULL_%28NOR%29.zip)) and extract the contents. If you have a NAND console, you will need to rename the .bin.minimal file to just .bin. Place the .bin file on the root of your USB device. Plug your USB device into the right-most slot on your PS3.

2. Open Rebug Toolbox and select "Resize VFLASH/NAND Regions". Petitboot will install.

3. Download Red Ribbon Linux (or other Linux flavor ported to PS3) and burn it to a disk or USB device using software such as [balenaEtcher](http://www.balena.io/etcher).

4. Open Rebug Toolbox and select "Boot OtherOS". Select "Apply Current" when it asks about LV1 Patches. Your PS3 will reboot and load Petitboot

5. Plug in a USB keyboard and mouse and insert your Linux CD or USB; it should appear as a Live option at the top of Petitboot. If it doesn't appear, restart your PS3 and go back to Step 4.

6. Your chosen Linux OS will boot up. 
 * If using Red Ribbon, select the "Install Red Ribbon" icon. Select your desired settings. When it prompts, select "Use Current Partitions", then "Mount Point Specification". Red Ribbon will format your USB Drive and will install itself on to it. This process may take 30 minutes or longer.