**WARNING: There is always a chance of bricking your console when flashing data to the NAND/NOR chip. Never flash to your console unless you have multiple valid backup dumps**

# Downgrading your Console with ProgSkeet 

To minimize the chance of bricking, do NOT skip any of the following sections. This process will use a ProgSkeet to downgrade your console to 3.55 official firmware to allow the installation of custom firmware. Check to make sure that your [console is downgrade compatible](https://www.reddit.com/r/ps3homebrew/wiki/how_to_hack). A manual for the ProgSkeet can be found [here](http://web.archive.org/web/20160512123145/http://www.ProgSkeet.com/downloads/ProgSkeet1.2-MANUAL.pdf).

# NAND or NOR?

You will need to check the model number on the back of your console and compare it to the chart below to determine if your console is NAND-based or NOR-based.

Model|Flash
:--|:--
CECH-A through CECH-G|NAND
CECH-H through CECH-Q|NOR
CECH-2000 through CECH-2XXX|NOR
CECH-3000+|Cannot downgrade


# Materials Needed

- ProgSkeet
    - A JTAG programmer such as Injectus if using a solderless clip or ProgSkeet 1.2 / 1.21 (to update the bitstream)

- NOR only: 20 AWG to 26 AWG wire (CAT5, CAT5e, and CAT6 Ethernet cable wires work perfectly)

- NAND only: 28-30 AWG wire

- Thermal paste (Arctic Silver 5 recommended)

- Soldering iron, a wire stripper or lighter, and tin solder

- Slim models only: Torx T8 screwdriver

- Fat models only: Torx T10 screwdriver

- Downgrading files pack found on [Mega](https://mega.nz/#!H5cFgaSJ!0klsHOl7ADGoXU6n6qlqkBpM32f_Ib_NlPpqq-0oS5M), [FileDropper](http://www.filedropper.com/ufpgv460), or [FileFactory](http://www.filefactory.com/file/54fh8w24dga5/U.F.P.G.%20V4.60.exe) (U.F.P.G. v4.60)

- Optional: 360clip (solderless), ProgSkeet NAND solderless adapter (NAND only) or a UniClip.

    56-pin is a NOR clip, 48-pin is a NAND clip

# Updating Bitstream (Injectus)

Only complete this section if your ProgSkeet came without being fully programmed, which is the case with a new 1.2 or 1.21, or if you are using a solderless clip.

1. Connect the FCC 15 pin from the ProgSkeet to the Injectus programmer.

2. Download and extract the [Infectus Programmer Package](http://www.ProgSkeet.com/forum/viewtopic.php?f=10&t=3948) to your desktop.

3. Connect USB cable from Injectus to the USB port of your PC. It will prompt you to install a driver. Select the driver located in the "USB Drivers 3.1" folder. 

4. Download the respective .DAT file (listed below)

    **ProgSkeet 1.0 / 1.1**

   • [ProgSkeet_Bitstreams_111106.rar](http://www.mediafire.com/?o66ls0yo8o1ybr8) (NOR+Clip OR NAND/NOR soldered)

   • [ProgSkeet_Bitstreams_111126.rar](http://www.mediafire.com/?h3dc7ohc2b2xon8) (NAND Clip only)

    **ProgSkeet 1.2 / 1.21**

   • [WinSkeet_130721_0313.rar](http://www.sendspace.com/file/kss22d) (NAND/NOR)


5. Run InfectusProgrammer_3.9.9.0.exe and click Tools → Open Infectus.

6. Select the .DAT file that you had downloaded and select the Program button.


# Soldering (NAND)

On the ProgSkeet board, two jumpers need to be bridged together with solder. The upper pads circled in yellow (R9 and R11) on [this image](http://web.archive.org/web/20160506162010/http://i.imgur.com/g3VRZ.png) need to be soldered with the 3.3V pads to look like [this](http://web.archive.org/web/20160506162124/http://i.imgur.com/MBseP.png). Ignore the red circle and **DO NOT remove R7 or R8** as other guides may recommend.

You will need to connect your ProgSkeet to the first NAND (Flash0) using the "A" side of the Y-Adapter.

If using a clip, you will need to solder a wire from the 3.3V pad on the Y-Adapter to the 3.3V pad on the ProgSkeet. If using a 360clip or ProgSkeet NAND solderless adapter, it can be plugged directly into the ProgSkeet. If using a UniClip, it must be soldered onto the ProgSkeet using [this diagram](http://web.archive.org/web/20160506162928/http://www.360-clip.com/UNI-CLIP-48-03.jpg). It is recommended to clean the pins on your clip with rubbing alcohol and a Q-tip before connecting it. Before attaching the clip sockets to the motherboard, check that there are no tiny components in the way that will prevent it from sitting flush; if there are, shave plastic off of the bottom of your chip until it will sit flush. Some motherboards require the shaving of an entire side of the clip to fit in place. 

If you are not using a clip, check around the edges of your motherboard to find the motherboard model number printed on the board. Click the link for your motherboard model and solder the contact points of the ProgSkeet to the corresponding contact point on the motherboard. You may have to use one of the following ProgSkeet diagrams to match the pins: [ProgSkeet 1.0/1.1](http://web.archive.org/web/20160511152500/http://www.consoleopen.com/forum/images/tutorial/Ps3/Downgrade_Ps3_NOR_Native_3.56/Nor_Retail_ProgSkeet_1.jpg), [ProgSkeet 1.2/1.21](http://web.archive.org/web/20160511152431/http://www.kingx.de/pic/img/ProgSkeet-1.2-Loetpunkte.PNG). You only need to solder to one GND point on the motherboard. 

[COK-001](http://web.archive.org/web/20160511122622/http://www.psdevwiki.com/ps3/images/5/52/COK-001_NAND_traces.jpg)

[COK-002 / COK-002W](http://web.archive.org/web/20160511122457/http://www.psdevwiki.com/ps3/images/7/7a/COK-002_NAND_traces.jpg)

[SEM-001](http://web.archive.org/web/20160511122742/http://www.psdevwiki.com/ps3/images/c/c5/SEM-001_NAND_traces.jpg)

* It is recommended to label the wires with masking tape or [these tabs](http://web.archive.org/web/20161212191810/http://i.imgur.com/XTGVXGS.png) to keep track of them.



# Soldering (NOR 1.0 / 1.1)

On the ProgSkeet board, two jumpers need to be bridged together with solder, and a resistor needs to be removed. The upper pads circled in yellow (R9 and R11) on [this image](http://web.archive.org/web/20160506162010/http://i.imgur.com/g3VRZ.png) need to be soldered with the 3.3V pads to look like [this](http://web.archive.org/web/20160506162124/http://i.imgur.com/MBseP.png). The resistor circled in red (R7) needs to be removed completely. **DO NOT remove R7 or R8** as other guides may recommend.

Check around the edges of your motherboard to find the motherboard model number printed on the board. Click the link for your motherboard model and solder the contact points of the ProgSkeet to the corresponding contact point on the motherboard. 

If using a 360clip or ProgSkeet NAND solderless adapter, it can be plugged directly into the ProgSkeet. If using a UniClip, it must be soldered onto the ProgSkeet using [this diagram](http://web.archive.org/web/20160506162928/http://www.360-clip.com/UNI-CLIP-48-03.jpg). It is recommended to clean the pins on your clip with rubbing alcohol and a Q-tip before connecting it. Before attaching the clip, check that there are no tiny components in the way that will prevent it from sitting flush; if there are, shave plastic off of the bottom of your chip until it will sit flush.


[DYN-001](http://web.archive.org/web/20160511132418/http://i.imgur.com/cynUEDp.png)

[VER-001](http://web.archive.org/web/20160511132546/http://i.imgur.com/NGiEaXX.png)

[DIA-001 & DIA-002](http://web.archive.org/web/20160511131302/http://i.imgur.com/OqToQpY.png) 

[JSD-001 & SUR-001 & JTP-001](http://web.archive.org/web/20160511132353/http://i.imgur.com/wdE1uKi.png)


# Soldering (NOR 1.2 / 1.21)

Remove the R7 bridge and solder the two R8 pads together to put the ProgSkeet in NOR mode. An image of this can be found [here](http://web.archive.org/web/20160511083106/http://i.imgur.com/mcp56MR.jpg). **DO NOT remove R8** as other guides may recommend.

Check around the edges of your motherboard to find the motherboard model number printed on the board. Click the link for your motherboard model and solder the contact points of the ProgSkeet to the corresponding contact point on the motherboard. 

If using a 360clip or ProgSkeet NAND solderless adapter, it can be plugged directly into the ProgSkeet. If using a UniClip, it must be soldered onto the ProgSkeet using [this diagram](http://web.archive.org/web/20160506162928/http://www.360-clip.com/UNI-CLIP-48-03.jpg). It is recommended to clean the pins on your clip with rubbing alcohol and a Q-tip before connecting it. Before attaching the clip, check that there are no tiny components in the way that will prevent it from sitting flush; if there are, shave plastic off of the bottom of your chip until it will sit flush.

[DYN-001](http://web.archive.org/web/20160511092809/http://i.imgur.com/6dAVI.jpg)

[VER-001](http://web.archive.org/web/20160511092701/http://i.imgur.com/xbvGe.jpg)

[DIA-001 & DIA-002](http://web.archive.org/web/20160511092813/http://i.imgur.com/WR8F9.jpg)

[JSD-001 & SUR-001 & JTP-001 & KTE-001](http://web.archive.org/web/20160511092730/http://i.imgur.com/0RBqi.jpg)

 
# Install the ProgSkeet Drivers
 
1. Install the [U.F.P.G. v4.60](https://mega.nz/#!H5cFgaSJ!0klsHOl7ADGoXU6n6qlqkBpM32f_Ib_NlPpqq-0oS5M) and select NAND/NOR ProgSkeet, regardless of number version. 

2. Install the ProgSkeet driver by running the WinSkeet icon.

3. Plug your ProgSkeet into your PC with your PS3 controller cable.

4. The device will be detected and the Install New Hardware wizard will run. Select "Not this time" if given the option.

5. Select "Install from a list or specific location" → Browse to Location → Select "C:\Users\<username>\Desktop\ProgSkeet 1.1  Programs\Setup Files\drivers_WinUSB_111121\" and finish installation.


# Taking Backup Dumps (NAND)

1. Connect your ProgSkeet to your PC via USB cable.

2. Browse to C:\Users\<username>\Desktop\ProgSkeet 1.1 NAND Programs\WinSkeet111205 and run WinSkeet40000.

3. Under the Presets section, select the drop-down menu and select Dual NAND.

4. Select the NAND tab, and enable the NAND 1 checkbox. 

5. Select the Auto button. It should automatically populate the NAND 1 fields. If it doesn't, check the connection of the clip or wires.

6. Select the Dump button. It will prompt you to save the backup. Name the backup "NAND Flash0 - 1". It will take about 12 minutes. Repeat the process two more times and name the new backups "NAND Flash0 - 2" and "NAND Flash0 - 3".

7. Unplug the ProgSkeet and connect the ProgSkeet to the second NAND (Flash1). Reconnect the ProgSkeet to your PC.

8. Enable the NAND 2 checkbox.

9. Select the Auto button. It should automatically populate the NAND 2 fields. If it doesn't, check the connection of the clip or wires.

10. Select the Dump button. It will prompt you to save the backup. Create a folder called "dumps" and enter it. Name the backup "NAND Flash1 - 1". It will take about 12 minutes. Repeat the process two more times and name the new backups "NAND Flash1 - 2" and "NAND Flash1 - 3".
 * If you receive verification errors, it may be due to incorrect wiring, use of 30AWG wire, wires being too long, a bad USB cable, interference, bad grounding, or bad luck. 

11. On your PC, browse to C:\Users\<username>\Desktop\ProgSkeet 1.1 NAND Programs\ and run FlowRebuilder v.4.2.2.0. Select "UNSCRAMBLE then interleave two NAND flashes into one unified dump". In the Flash 0 field, browse to your dumps folder and select "NAND Flash0 - 1". In the Flash 1 field, browse to your dumps folder and select "NAND Flash1 - 1". Under the "Select the OUTPUT (interleaved) file", browse to your dumps folder, create a new folder called "extracted" and enter it; name the file as "dump 1". Select Execute Operation. Repeat this process with the two other NAND dump sets, changing the output file to "dump 2", and finally "dump 3". Verify that there are now three files located in the extracted folder. If you are missing any, try to join the dumps again. If they still are missing, you will need to redo all of the dumps completely.


# Taking Backup Dumps (NOR)

1. Connect your ProgSkeet to your PC via USB cable.

2. Browse to C:\Users\<username>\Desktop\ProgSkeet 1.1 NOR Programs\WinSkeet111205 and run WinSkeet40000.

3. Under the Presets section, select the drop-down menu and select the model number of your NOR chip, or select Dual NAND. You can find the model number of the NOR by looking on top of the chip on the motherboard.

4. Select the NOR tab and click Take Over. If this button is not present, check your USB cable connection and click Detect.

5. **Attach console fan and heat sinks attached back onto your motherboard if they were taken off, and plug the fan power cable in**. Turn on your PS3, it should halt during boot up. If it doesn't, turn your console back off and back on and it should halt.

6. Select "DUMP CFI" and save it as a CFI dump. This will verify your connection to the NOR. If it fails, check your wiring and make sure you have the right NOR model selected in the Common tab.

7. Select the Dump button. It will prompt you to save the backup. Create a folder called "dumps" and enter it. Name the backup "NOR - 1". It will take about 12 minutes. Repeat the process two more times and name the new backups "NOR- 2" and "NOR - 3".

* If you receive verification errors, it may be due to incorrect wiring, use of 30AWG wire, wires being too long, a bad USB cable, interference, bad grounding, or bad luck. 


# Verifying your Dumps

1. Download [Swizzy's Dump Checker](https://github.com/Swizzy/PS3DumpChecker/archive/master.zip) and extract it to your Desktop.

2. Drag your backup over the file "ps3_dump_checker.exe". The program will open and validate your dump.

3. Click "No" if it asks if you want to patch the dump.

4. Ensure that it reports "OK". If it doesn't, check the left hand side to find out what tests it failed. If the only failed tests are some combination of ROS0, ROS1, TRVK_PKG0 Hash, and TRVK_PKG1 Hash; click the wrench in the top left, disable Hash Checks, and try and validate the dump again. If any other tests are failed and you are using a clip, try re-seating the clip or putting a stationary object on top of the clip (no heavier than a baseball), and taking another set of backups. Once you have a valid backup, you may proceed.


# Patching and Flashing (NAND)

1. Drag the first backup over "ps3_dump_checker.exe" again, this time saying "Yes" when it asks if you want to patch the dump. A new file named NAND_patched.bin or NOR_patched.bin will be generated.

2. The patched dump will need to be split by opening FlowRebuilder again. Select "RE-SCRAMBLE a modified dump then de-interleave it into two new flashes". Select your original Flash0 and Flash1 dumps, as well as the "NAND_patched.bin" dump. Select Execute. This will create two new files called "NAND Flash0.new.bin" and "NAND Flash1.new.bin". 

3. Ensure the ProgSkeet is still properly connected to the PC and the PS3 motherboard.

4. Open WinSkeet and select your NAND model in the drop-down. 

5. Select the NAND tab, make sure Flash1 is checked, and click “Dump CFI” to ensure that the NAND is connected properly. 

6. Select the Flash button and choose "NAND Flash1.new.bin". It should automatically read, erase, flash, and verify the NAND chip. This process will take approximately 19 minutes and should say "Nothing to flash!" and "Finished" when done. 
 * If you have an address that will not verify, change the bottom drop-down option to "USB transfer timing (avoid)", wait for it to finish processing, and retry. Ensure that your wires are not touching any bare metal of the case. If you still have issues, try bridging GP4 and RDY together on the ProgSkeet.

7. Turn off the PS3, unplug your ProgSkeet from your PC, disconnect your ProgSkeet from the PS3. Reconnect your ProgSkeet to the first NAND (Flash0), then plug your ProgSkeet back into the PC.

8. Select the NAND tab, make sure Flash0 is checked, and click “Dump CFI” to ensure that the NAND is connected properly. 

9. Select the Flash button and choose "NAND Flash0.new.bin". It should automatically read, erase, flash, and verify the NAND chip. This process will take approximately 19 minutes and should say "Nothing to flash!" and "Finished" when done. 
 * If you have an address that will not verify, change the bottom drop-down option to "USB transfer timing (avoid)", wait for it to finish processing, and retry. Ensure that your wires are not touching any bare metal of the case. If you still have issues, try bridging GP4 and RDY together on the ProgSkeet.

10. Turn off the PS3, unplug your ProgSkeet from your PC, disconnect your ProgSkeet from the PS3.

11. **Attach console fan and heat sinks attached back onto your motherboard if they were taken off, and plug the fan power cable in**. Turn the PS3 back on. Depending on your firmware version, your PS3 may boot to recovery mode, or straight to the XMB. Do not panic if it boots to recovery mode. If you make it to this point, your console successfully took the patched dump. If it did not, try reflashing again.

12. Follow the [instructions to install CFW](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw) or follow [this guide](https://www.reddit.com/r/ps3homebrew/wiki/general_setup) for a recommendation of firmware and applications. You can go directly to a 4.XX CFW. If you are looking to go to a 3.XX firmware, make sure to use Rogero or Rebug "Downgrader" firmware, then your desired firmware. Keep in mind that if your minverchk reported "3.56" as the minimum, you can not install a 3.55 firmware.


# Patching and Flashing (NOR)

1. Drag the first backup over "ps3_dump_checker.exe" again, this time saying "Yes" when it asks if you want to patch the dump. A new file named NAND_patched.bin or NOR_patched.bin will be generated.

2. Ensure the ProgSkeet is still properly connected to the PC and the PS3 motherboard.

3. Open WinSkeet and select your NAND/NOR model in the drop-down. 

4. Select the NOR tab and click “Dump CFI” to ensure that the NOR is connected properly. 

5. At the bottom of the window under the Options section, change the settings as according to your NAND/NOR model:

    **Spansion S29GL128N90TFIR2**

    Buffered write (fastest, default)

    Ready triggered timing (fastest, default)

    Max bytes: 32 (or 16)

    \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-

    **Samsung K8Q2815UQB-PI4B**

    Single word program

    Ready triggered timing (fastest, default)

    Max bytes: (greyed out by single word program)

    \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-

    **Spansion S29GL128P90TFIR2** 

    Buffered write (fastest, default)

    Ready triggered timing (fastest, default)

    Max bytes: 64 (or 32)

    \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-

    **Samsung K8P2716UZC-QI4D**

    Buffered write (fastest, default)

    Ready triggered timing (fastest, default)

    Max bytes: 64 (or 32)

    \-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-

    **Macronix MX29GL128ELT2I-90G**  

    Buffered write (fastest, default)

    Ready triggered timing (fastest, default)

    Max bytes: 64 (or 32)


6. Select the Flash button and choose "NAND Flash0.new.bin" or "NOR_patched.bin". It should automatically read, erase, flash, and verify the NOR chip. It should say "Nothing to flash!" and "Finished" when done. If you have an address that will not verify, change the bottom drop-down option to "USB transfer timing (avoid)", wait for it to finish processing, and retry. Ensure that your wires are not touching any bare metal of the case. If you still have issues, try bridging GP4 and RDY together on the ProgSkeet.

7. Turn off the PS3, unplug your ProgSkeet from your PC, disconnect your ProgSkeet from the PS3.
 
8. **Attach console fan and heat sinks attached back onto your motherboard if they were taken off, and plug the fan power cable in**. Turn the PS3 back on. Depending on your firmware version, your PS3 may boot to recovery mode, or straight to the XMB. Do not panic if it boots to recovery mode. If you make it to this point, your console successfully took the patched dump. If it did not, try reflashing again and make sure you used the right Diff file.

7. Follow the [instructions to install CFW](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw) or follow [this guide](https://www.reddit.com/r/ps3homebrew/wiki/general_setup) for a recommendation of firmware and applications. You can go directly to a 4.XX CEX or REX CFW that is of an equal or higher number to the OFW version you are on. If you are looking to go to a lower firmware, make sure to use Rogero or Rebug "Downgrader" firmware, then your desired firmware. **Keep in mind that if your minverchk reported "3.56" as the minimum, do not install a 3.55 or lower firmware**.

# Bad Flash Recovery

In the event that something goes wrong, and your console is not working properly (or "bricked"), you may be able to recover it. First try flashing the patched dump again. If that doesn't work and you have your original backup dump from the "Taking Backup Dumps" section above, flash the backup dump to your console. If you have a NOR console and your PS3 won't stay on, you must solder a wire between the TRISTATE point and a GND connection on your motherboard; you will need to remove this after flashing. You may be able to get away with taping a wire down or having someone hold one to the points if you do not have soldering tools.

* If you still can't get a good dump, you can try and modify someone else's dump to work with your console. Once you obtain someone else's NAND/NOR dump, you will have to open it up with a hex editor such as [HxD](https://mh-nexus.de/en/downloads.php) and compare it with yours. You will need to copy information marked as red on this chart ([NAND](https://web.archive.org/web/20141119050029/http://www.psdevwiki.com/ps3/Flash#NAND_Flash)/[NOR](https://web.archive.org/web/20141119050029/http://www.psdevwiki.com/ps3/Flash#NOR_Flash)) from your backup to the other one to construct a working one. Hopefully, you have enough information that the dump checker will consider it as a valid dump.
