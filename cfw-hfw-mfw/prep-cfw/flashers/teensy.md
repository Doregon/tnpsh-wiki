**WARNING: There is always a chance of bricking your console when flashing data to the NAND/NOR chip. Never flash to your console unless you have multiple valid backup dumps**

# Downgrading your Console with Teensy

To minimize the chance of bricking, do NOT skip any of the following sections. This process will use a Teensy to downgrade your console to 3.55 official firmware to allow the installation of custom firmware. Check to make sure that your [console is downgrade compatible](https://www.reddit.com/r/ps3homebrew/wiki/how_to_hack).

# NAND or NOR?

You will need to check the model number on the back of your console and compare it to the chart below to determine if your console is NAND-based or NOR-based.

Model|Flash
:--|:--
CECH-A through CECH-G|NAND
CECH-H through CECH-Q|NOR
CECH-2000 through CECH-2XXX|NOR
CECH-3000+|Cannot downgrade


Materials Needed
---
* [Teensy++ 2.0](http://www.pjrc.com/store/teensypp_pins.html)

* [One set of extra header pins](http://www.pjrc.com/store/header_12x1.html) for the center points on the Teensy

* [3.3V voltage regulator](http://www.pjrc.com/store/mcp1825.html) if powering from USB

* NOR only: 20 AWG to 26 AWG wire (26 AWG recommended; Ethernet cable wires work great) **OR** [female jumper wires](https://www.amazon.com/s/field-keywords=female%20jumper%20wires) which eliminate the need to solder on your Teensy

* NAND only: 28-30 AWG wire **OR** [female jumper wires](https://www.amazon.com/s/field-keywords=female%20jumper%20wires) which eliminate the need to solder on your Teensy

* Slim models only: Torx T8 screwdriver

* Fat models only: Torx T10 screwdriver

* Thermal paste (Arctic Silver 5 recommended)

* Razor blade (such as an Xacto knife)

* Soldering iron, a wire stripper or lighter, and tin solder

* Optional: 360clip or UniClip


    56-pin is a NOR clip, 48-pin is a NAND clip


* Optional: Flux or rosin-core solder for less impurities and better solder control, and magnifying glasses


Checking Authenticity
---
* Read [this page](https://web.archive.org/web/20160315232235/https://www.pjrc.com/teensy/counterfeit.html) to ensure that your Teensy is from a reliable source and is not a counterfeit product. If you suspect your Teensy is a fake, immediately attempt a return and buy a new one from a trusted vendor.

# Setting up your PC

1. Download, extract, and install the [CoolShrimp's Downgrade Tool v1.03](http://www.mediafire.com/file/f32netyd3phn5e1/Downgrade_Tool_%2528PS3%2529_v1.03_Setup.rar/file).

2. Run the newly installed "PS3 Downgrade Tool". Select the Settings tab, and run the installers for Python, pySerial, and the Teensy 2++ Driver. Run the "Flash for NAND" if your console is NAND-based or "Flash for NOR" installer if your console is NOR-based.

3. From the Settings tab, click "Show Device Manager", expand Ports, and you should see "USB serial (Communication Class Abstract Control Model) (COM#)". Take note of the COM number at the end of the name, and select this COM number from the drop-down menu under the "Show Device Manager" button.

 * If you have issues with drivers, especially on Windows 10, see [these official instructions](http://web.archive.org/web/20160201055204/http://www.pjrc.com/teensy/windows8.txt)

Setting up Power
---

We will need to modify the Teensy so that it does not provide too much power to the NAND/NOR and fry it. Use the pictures provided in the [official documentation](https://web.archive.org/web/20160127053304/https://www.pjrc.com/teensy/3volt.html) to assist you.

* Using picture 3 as reference, use a razor to cut the connection between the pads next to where it says "5V". If you apply a tiny bit of rubbing alcohol, you'll be able to see the trace more clearly while cutting. The cut does not have to be very deep, but be careful not to cut any other components. A magnifying glass may be helpful at this point.

* Follow one of these options to power the device:

## Using USB Power 

* Using pictures 1 and 2 as reference, solder the 3.3V voltage regulator into place on the Teensy.


## Using the Motherboard Power

* Using picture 4 as reference, solder the two pads next to where it says "3V" together on the Teensy.


# Soldering Extra Pins

Using pliers on your [extra header pins](http://www.pjrc.com/store/header_12x1.html), break away two sets of 4 pins, and one set of 2 pins. With the two large rows of pins facing up, place the short side of the extra pins into the holes in the center of the Teensy, and solder them in place. They should look just like the two built-in rows of pins. Repeat the process for the set of 2 pins.  


# Soldering (NOR)

Check around the edges of your motherboard to find the motherboard model number printed on the board. Click the link for your motherboard model and solder the contact points of the Teensy to the corresponding contact point on the motherboard. Only solder the 3.3V point to VCC if you plan on powering your Teensy off of the motherboard power, meaning you did *not* install a voltage regulator. You only need to solder to one GND point on the motherboard. If you are using female jumper wires, cut one end off of the wires to solder onto the PS3 and plug the other end into the Teensy.

If using a clip, see the respective diagram: [NOR 360clip](http://web.archive.org/web/20160506162659/http://i.imgur.com/zwxI43O.jpg), [UniClip](http://web.archive.org/web/20160506162716/http://i.imgur.com/8iONJT1.jpg). It is recommended to clean the pins on your clip with rubbing alcohol and a Q-tip before soldering it. Before attaching the clip, check that there are no tiny components in the way that will prevent it from sitting flush; if there are, shave plastic off of the bottom of your chip until it will sit flush.


[DYN-001](http://web.archive.org/web/20160506162751/http://i.imgur.com/0sRBP27.jpg)

[VER-001](http://web.archive.org/web/20160506162805/http://i.imgur.com/ixhtNlI.jpg)

[DIA-001 & DIA-002](http://web.archive.org/web/20160506162737/http://i.imgur.com/LIPsrW3.jpg)

[JSD-001 & SUR-001 & JTP-001](http://web.archive.org/web/20160506162853/http://i.imgur.com/MPJZIc6.jpg)

* It is recommended to label the wires with masking tape or [these tabs](http://web.archive.org/web/20161212191810/http://i.imgur.com/XTGVXGS.png) to keep track of them.


# Soldering (NAND)

Check around the edges of your motherboard to find the motherboard model number printed on the board. Click the link for your motherboard model and solder the contact points of the Teensy to the corresponding contact point on the motherboard. You will be soldering to the Flash0 first. Only solder the 3.3V point to VCC if you plan on powering your Teensy off of the motherboard power, meaning you did *not* install a voltage regulator. You only need to solder to one GND point on the motherboard. If you are using female jumper wires, cut one end off of the wires to solder onto the PS3 and plug the other end into the Teensy.

If using a clip, see the respective diagram: [NAND 360clip](http://web.archive.org/web/20160511145513/http://www.360-clip.com/Nand_Diagram_for-progskeet.jpg), [UniClip](http://web.archive.org/web/20160506162928/http://www.360-clip.com/UNI-CLIP-48-03.jpg). It is recommended to clean the pins on your clip with rubbing alcohol and a Q-tip before soldering it. Before attaching the clip, check that there are no tiny components in the way that will prevent it from sitting flush; if there are, shave plastic off of the bottom of your chip until it will sit flush.


[COK-001](http://web.archive.org/web/20160511122622/http://www.psdevwiki.com/ps3/images/5/52/COK-001_NAND_traces.jpg)

[COK-002 / COK-002W](http://web.archive.org/web/20160511122457/http://www.psdevwiki.com/ps3/images/7/7a/COK-002_NAND_traces.jpg)

[SEM-001](http://web.archive.org/web/20160511122742/http://www.psdevwiki.com/ps3/images/c/c5/SEM-001_NAND_traces.jpg)

* It is recommended to label the wires with masking tape or [these tabs](http://web.archive.org/web/20161212191810/http://i.imgur.com/XTGVXGS.png) to keep track of them.


#Taking Backup Dumps

1. Right click and run the Downgrade Tool as administrator on your PC, and select the "Nand" tab.

2. **Attach console fan and heat sinks attached back onto your motherboard if they were taken off, and plug the fan power cable in**. Turn on your PS3, and then plug your Teensy into your PC.

3. Under Step 1, select NAND or NOR, and any function in the drop-down in under the Write Mode area (do not leave this blank).

4. Select "Check Connection" under Step 2. It should open a Command Prompt and tell you the NOR chip type (if it's a NOR model), or the available memory (if it's a NAND model). If you do not see either, make sure your connections are good and that bare wire isn't touching any metal it's not supposed to be touching.

5. Press any key to close the window, then click "Read Nand" under Step 3. It should tell you the NAND/NOR type, and say "Dumping". If you see any errors, stop the dump and try reseating the clip or checking your soldering to make sure you soldered them correctly. It will take approximately 1 minute on a NOR console, and 20 minutes on a NAND console before seeing the confirmation message "Done" when completed.

6. Press any key to continue, then save the dump on your PC and name it "NAND Flash0" or "NOR".

7. (NAND ONLY): Disconnect your connection from the first NAND (Flash0), and attach your clip or solder onto the second NAND (Flash1). Repeat the above steps to obtain a dump of the second NAND and name it "NAND Flash1". The two dumps will need to be joined by clicking "Join/Split NANDs" within Downgrade Tool, and selecting "UNSCRAMBLE and interleave two NAND flashes into one unified dump". Save the dump as "merged.bin" and click Execute. This will also create a folder with the files of the dump extracted, named "merged.ext". If you do not see the .ext folder, try joining them again, but swapping the top and bottom dumps and **take note that you did this**. If it still does not show up, you will need to get new dumps.

# Verifying your Dumps

1. Download [Swizzy's Dump Checker](https://github.com/Swizzy/PS3DumpChecker/archive/master.zip) and extract it to your Desktop.

2. Drag your backup over the file "ps3_dump_checker.exe". The program will open and validate your dump.

3. Click "No" if it asks if you want to patch the dump.

4. Ensure that it reports "OK". If it doesn't, check the left hand side to find out what tests it failed. If the only failed tests are some combination of ROS0, ROS1, TRVK_PKG0 Hash, and TRVK_PKG1 Hash; click the wrench in the top left, disable Hash Checks, and try and validate the dump again. If any other tests are failed and you are using a clip, try re-seating the clip or putting a stationary object on top of the clip (no heavier than a baseball), and taking another set of backups. Once you have a valid backup, you may proceed.

# Patching and Flashing

1. Drag the first backup over "ps3_dump_checker.exe" again, this time saying "Yes" when it asks if you want to patch the dump. A new file named NAND_patched.bin or NOR_patched.bin will be generated.

2. Right click and run the Downgrade Tool as administrator on your PC, and select the "Nand" tab.

    (NAND ONLY): The patched dump will need to be split by clicking "Join/Split NANDs" within Downgrade Tool, and selecting "RE-SCRAMBLE a modified dump then de-interleave it into two new flashes". Select your original top and bottom dump, as well as the "NAND_patched.bin" dump. If you had to swap the top and bottom dumps when you joined them, **do so again now**. Finally, select Execute. This will create two new files called "NAND Flash0.new.bin" and "NAND Flash1.new.bin".

3. Ensure the Teensy is still properly connected to the PC and the PS3 motherboard, with the Teensy receiving power.

4. (NOR ONLY) Under Step 1, select NOR, and "Write" in the drop-down in under the Write Mode area.

    (NAND ONLY) Under Step 1, select NAND, and "DiffWrite" in the drop-down in under the Write Mode area.

5. Select "Check Connection" under Step 2. It should open a Command Prompt and tell you the NOR chip type (if it's a NOR model), or the available memory (if it's a NAND model). If you do not see either, make sure your connections are good and that bare wire isn't touching any metal it's not supposed to be touching. Press any key to close the window.

6. (NOR ONLY) Click "Write to NAND" (this is not a typo in this guide) under Step 6. Select "NOR_patched.bin".

    (NAND ONLY) Click "Write to NAND" under Step 6. Select "NAND Flash1.new.bin". It will then ask for a diff file. Select the "DifferentialFileFlash1.txt" located in the "NANDway Programs/Dumps/Differential Flashing" folder.

7. A Command Prompt window will open and it should tell you the NAND/NOR type, and should confirm that it is writing. If you see any errors, stop the flash and try reseating the clip or checking your soldering to make sure you soldered them correctly. It will take about 2 to 5 minutes and it will say "Done" when completed. 
 
    (NAND ONLY): Attach the Teensy to the first NAND (Flash0) and write the patched NAND file using DifferenceFileFlash0. It recommended to take a test dump and [compare it's MD5 hash](https://www.reddit.com/r/ps3homebrew/wiki/md5) to your original dump, just to make sure you have a perfect connection.

8. Detach the D6 pin on the Teensy (as well as any connection you may have to the TRISTATE point for NOR consoles) and rebuild the console to the point that everything – including the Blu-Ray drive and the HDD – is plugged in and you've applied a new coat of thermal paste with the fans and heatsinks attached. If the D6 pin and TRISTATE connection (NOR only) is not removed, you will not be able to install new firmware to your console (error 8002F14E).

9. **Attach console fan and heat sinks attached back onto your motherboard if they were taken off, and plug the fan power cable in**. Turn the PS3 back on. Depending on your firmware version, your PS3 may boot to recovery mode, or straight to the XMB. If you make it to this point, your console successfully took the patched dump and you can remove the Teensy if desired. If it did not, try reflashing again and make sure you used the right Diff file.

7. Follow the [instructions to install CFW](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw) or follow [this guide](https://www.reddit.com/r/ps3homebrew/wiki/general_setup) for a recommendation of firmware and applications. You can go directly to a 4.XX CEX or REX CFW that is of an equal or higher number to the OFW version you are on. If you are looking to go to a lower firmware, make sure to use Rogero or Rebug "Downgrader" firmware, then your desired firmware. **Keep in mind that if your minverchk reported "3.56" as the minimum, do not install a 3.55 or lower firmware**.

# Bad Flash Recovery

In the event that something goes wrong, and your console is not working properly (or "bricked"), you may be able to recover it. First try flashing the patched dump again. If that doesn't work and you have your original backup dumps from the "Taking Backup Dumps" section above, flash the backup dump to your console. If you have a NOR console and your PS3 won't stay on, you must solder a wire between the TRISTATE point and a GND connection on your motherboard; you will need to remove this after flashing. You may be able to get away with taping a wire down or having someone hold one to the points if you do not have soldering tools.

* If you still can't get a good dump, you can try and modify someone else's dump to work with your console. Once you obtain someone else's NAND/NOR dump, you will have to open it up with a hex editor such as [HxD](https://mh-nexus.de/en/downloads.php) and compare it with yours. You will need to copy information marked as red on this chart ([NAND](https://web.archive.org/web/20141119050029/http://www.psdevwiki.com/ps3/Flash#NAND_Flash)/[NOR](https://web.archive.org/web/20141119050029/http://www.psdevwiki.com/ps3/Flash#NOR_Flash)) from your backup to the other one to construct a working one. Hopefully, you have enough information that the dump checker will consider it as a valid dump.
