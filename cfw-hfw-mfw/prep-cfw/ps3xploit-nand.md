# ps3xploit \(NAND\)

**WARNING: There is always a chance of bricking your console when flashing data to the NAND/NOR chip.**

## Exploiting your Console using PS3Xploit

To minimize the chance of bricking, do NOT skip any of the following sections. This process will use a recently released software hack to to allow the installation of custom firmware. Check to make sure that your [console is downgrade compatible](https://www.reddit.com/r/ps3homebrew/wiki/how_to_hack).

**With any newly released exploit of this calibur, there is always a chance that you can brick your console. Follow all sections of this guide exactly as how they are written.**

## NAND or NOR?

It is recommended to check the model number on the back of your console and compare it to the chart below to determine if your console is NAND-based or NOR-based. If your console is not NAND based, go back to the [How to Hack](https://www.reddit.com/r/ps3homebrew/wiki/how_to_hack) page and choose a different guide.

| Model | Flash |
| :--- | :--- |
| CECHA through CECHG | NAND |
| CECHH through CECHQ | NOR |
| CECH-2000 through CECH-25XX | NOR |
| CECH-3000+ | Cannot downgrade |

## Materials Needed

* A USB storage device, **formatted as FAT32 with 32kb allocation size**
* [NOR/NAND Flash Writer zip file](http://ps3xploit.com/hfw/release/NOR_NAND_writer_release_2.0.2_PS3Xploit.zip) \(extracted on Desktop\)
* ps3\_dump\_checker.exe from [Edythator's version of Swizzy's Dump Checker](https://github.com/Edythator/PS3DumpChecker/archive/master.zip)
* [4.85.1 HFW .PUP](https://mega.nz/#!SAYhnYYB!6CmxOz0H_pSuVRb4YZ7-lYvY66hP0LlohgVMWfFut4Q)

## \(Method 1\) Using an Exploit-Loading Site

1. Double check that [your console is a NAND console, and not a NOR console](https://www.reddit.com/r/ps3homebrew/wiki/ps3xploit_nand#wiki_nand_or_nor.3F). **You will risk bricking your console if it is a NOR console!**
2. Ensure your USB drive is formatted as FAT32, and that it is recognized by your PS3 by checking that it shows up on the XMB under Photos, Music, or Videos column.
3. Plug the USB drive into your computer, and copy over the "flash\_485.hex" file to the root of the drive.
   * [Verify the MD5 checksum](https://reddit.com/r/ps3homebrew/wiki/md5) of this file matches the checksum:  `2D74B066E7453E6B1336E36C410FB1EB` before continuing. If they match, you may continue, otherwise you will need to redownload the NOR/NAND Flash Writer zip file and verify again.
4. Update to 4.85.1 HFW using [this guide](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw) and the .PUP linked in the "Materials Needed" section.
   * [Verify the MD5 checksum](https://reddit.com/r/ps3homebrew/wiki/md5) of the PUP matches the checksum:  `C6632994C04D0ED8C555091F3FDE9BBB` before continuing. If they match, you may continue, otherwise you will need to redownload the PUP and verify again.
5. Plug the USB drive into the right-most USB port.
6. Navigate to the Network column of the XMB and select "Internet Browser". Press Start and enter the URL for the PS3Xploit website: `http://ps3xploit.com/hfw/writer/index_nand.html`. You should receive a message indicating that your console is compatible. If you do not, reinstall 4.85.1 HFW. Press Cross to dismiss the compatibility message.
7. Press Triangle, scroll down one option and select Tools → Home Page. Scroll down two options to "Use Current" and press Cross. Scroll down to OK and press Cross to exit this menu.
8. Press Circle and choose Yes to exit the browser.
9. Launch the Internet Browser again. Read the warnings on screen, and ensure that the `/dev_usb000/flash_485.hex` option is checked.
10. Hover over the "Initialize exploitation" button and press Cross. A success message should almost instantly appear indicating "Exploit Initialization SUCCESS...!". If it fails, follow the on-screen instructions to refresh the page.
11. Select "Patch NAND Flash Memory". A message should appear saying "Proceeding to patch NAND Flash Memory...". After a few minutes, it should change to "NAND Flash memory patch operation completed..!". If it takes longer than 5 minutes to complete, exit the browser and try again.
12. On the PS3, navigate to `http://ps3xploit.com/hfw/dumper/index_nand.html`. Press Triangle, scroll down one option and select Tools → Home Page. Scroll down two options to "Use Current" and press Cross. Scroll down to OK and press Cross to exit this menu.
13. Press Circle and choose Yes to exit the browser.
14. Launch the Internet Browser again. Read the warnings on screen, and ensure `/dev_usb000/dump.hex` is selected, click the "Initialize exploitation" button, wait for a success message, and then choose "Dump 239MB NAND to USB/Card device" and wait until you receive a message saying "NAND Flash dump operation completed..!".
    * If it takes longer than 30 minutes, try another USB storage device.
15. Unplug your USB storage device and plug it into your PC. Drag your dump.hex file over the file "ps3\_dump\_checker.exe". The program will open and validate your dump. If the dump comes up as "OK" it's okay to proceed. If it comes up as "BAD" and lists the only failures as the ROS0/ROS1 hash, you're okay to proceed.
    * If you receive a message saying that it is the wrong file size, you likely have a NOR console and not a NAND console. [Check again here](https://www.reddit.com/r/ps3homebrew/wiki/ps3xploit_nand#wiki_nand_or_nor.3F).
    * If you receive an error for only SKUIdentityData \(and maybe also ROS0 or ROS1\), your console is likely refurbished and it is okay to proceed.
    * **BACKUP THE DUMP.HEX FILE IF IT IS "OK"... SHOULD YOU MANAGE TO BRICK YOUR PS3, THIS FILE WILL BE USED WITH A HARDWARE FLASHER TO RESTORE THE CONSOLE**
16. Restart your console and proceed to install a CFW of equal or higher version with the ["Installing a CFW"](https://www.reddit.com/r/ps3homebrew/wiki/ps3xploit_nand#wiki_installing_a_cfw) instructions found below.

## \(Method 2\) Self-hosting the Exploit

These steps are an alternative to using an exploit-loading site.

1. Double check that [your console is a NAND console, and not a NOR console](https://www.reddit.com/r/ps3homebrew/wiki/ps3xploit_nand#wiki_nand_or_nor.3F). **You will risk bricking your console if it is a NOR console!**
2. Update to 4.85.1 HFW using [this guide](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw) and the .PUP linked in the "Materials Needed" section.
   * [Verify the MD5 checksum](https://reddit.com/r/ps3homebrew/wiki/md5) of the PUP matches the checksum:  `C6632994C04D0ED8C555091F3FDE9BBB` before continuing. If they match, you may continue, otherwise you will need to redownload the PUP and verify again.
3. Extract the NOR/NAND Flash Writer zip file into a folder labeled "NANDFlasher".
4. Inside of the NANDFlasher folder, create a folder called "htdocs".
5. Move the "ps3xploit\_writer\_v201.js", and the "index\_nand.html" files into htdocs, then rename "index\_nand.html" to "index.html".
6. Ensure your PS3 is connected to the same network as your PC, in order to be able to connect to the web server. This can either be through WiFi or network cables to your router.
7. Move the "miniweb.exe" file into the NANDFlasher folder and run it. This will start the web server on your local network.
8. Plug the USB drive into your computer, and copy over the "flash\_484.hex" file to the root of the drive and then plug it in the right-most USB port on the PS3.
9. Turn your PS3 off, then turn it back on again.
10. Navigate to the Network column of the XMB and select "Internet Browser". Press Start and enter the IP address and port that the miniweb window displays \(example: "192.168.11.010:1337"\). You should receive a message indicating that your console is compatible. If you do not, reinstall 4.85.1 HFW. Press Cross to dismiss the compatibility message.
11. Press Triangle, scroll down one option and select Tools → Home Page. Scroll down two options to "Use Current" and press Cross. Scroll down to OK and press Cross to exit this menu. Press Circle and choose Yes to exit the browser.
12. Launch the Internet Browser again. Read the warnings on screen, and ensure that the `/dev_usb000/flash_484.hex` option is checked.
13. Hover over the "Initialize exploitation" button and press Cross. A success message should almost instantly appear indicating "Exploit Initialization SUCCESS...!". If it fails, follow the on-screen instructions to refresh the page.
14. Select "Patch NAND Flash Memory". A message should appear saying "Proceeding to patch NAND Flash Memory...". After a few minutes, it should change to "NAND Flash memory patch operation completed..!". If it takes longer than 5 minutes to complete, exit the browser and try again.
15. On the PS3, navigate to `"192.168.11.010:1337"/index_nand.html`. Note the example IP we used from earlier. Press Triangle, scroll down one option and select Tools → Home Page. Scroll down two options to "Use Current" and press Cross. Scroll down to OK and press Cross to exit this menu.
16. Press Circle and choose Yes to exit the browser.
17. Launch the Internet Browser again. Read the warnings on screen, and ensure `/dev_usb000/dump.hex` is selected, click the "Initialize exploitation" button, wait for a success message, and then choose "Dump 239MB NAND to USB/Card device" and wait until you receive a message saying "NAND Flash dump operation completed..!".
    * If it takes longer than 30 minutes, try another USB storage device.
18. Unplug your USB storage device and plug it into your PC. Drag your dump.hex file over the file "ps3\_dump\_checker.exe". The program will open and validate your dump. If the dump comes up as "OK" it's okay to proceed. If it comes up as "BAD" and lists the only failures as the ROS0/ROS1 hash, you're okay to proceed.
    * If you receive a message saying that it is the wrong file size, you likely have a NOR console and not a NAND console. [Check again here](https://www.reddit.com/r/ps3homebrew/wiki/ps3xploit_nand#wiki_nand_or_nor.3F).
    * If you receive an error for only SKUIdentityData \(and maybe also the ROS0 hash or ROS1 hash\), your console is likely refurbished and it is okay to proceed.
    * **BACKUP THE DUMP.HEX FILE IF IT IS "OK"... SHOULD YOU MANAGE TO BRICK YOUR PS3, THIS FILE WILL BE USED WITH A HARDWARE FLASHER TO RESTORE THE CONSOLE**
19. Restart your console and proceed to install a CFW of equal or higher firmware version with the ["Installing a CFW"](https://www.reddit.com/r/ps3homebrew/wiki/ps3xploit_nand#wiki_installing_a_cfw) instructions found below.

## Bad Flash Recovery

In the event that something goes wrong while flashing your NAND, and your console is not working properly \(or "bricked"\), you may be able to recover it by updating the firmware normally through the XMB, ensuring you haven't shut down your console. Otherwise you can possibly boot into [recovery mode](https://www.reddit.com/r/ps3homebrew/wiki/recovery) and reinstall your current firmware from there. If this does not work, you will need to use a a hardware flasher to reflash. Please see Bad Flash Recovery section of the [E3](https://www.reddit.com/r/ps3homebrew/wiki/flashers/e3#wiki_bad_flash_recovery), [Teensy](https://www.reddit.com/r/ps3homebrew/wiki/flashers/teensy#wiki_bad_flash_recovery) or [ProgSkeet](https://www.reddit.com/r/ps3homebrew/wiki/flashers/progskeet#wiki_bad_flash_recovery) guides.

