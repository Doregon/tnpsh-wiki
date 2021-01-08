#ProDG Target Manager and Debugger (TMAPI)
___
ProDG (pronounced "prodigy"), also known as TMAPI, is the official tool used by PS3 developers to debug PS3 software. It can be used to view and modify values of variables on running programs on your console. It can be used for real time modding (RTM) as well as basic debugging. Note that in order to modify games, you must first convert their EBOOT to a [debug EBOOT](https://www.reddit.com/r/ps3homebrew/wiki/eboots). ProDG is supported only on DEX firmwares.

___

Setting up your PS3 for Debugging
---

Go to the settings column on the XMB menu and go all the way to the bottom to "Debug Settings" and make sure all the following setting are selected:

* Release Check Mode: Development Mode

* Boot Mode: System Software Mode

* Network Settings for Debug: Single Setting

If Debug Settings is not present, highlight "Network Settings" on the XMB and press and hold: Dpad-down + L1 + L2 + R1 + R2 + L3

Setting up ProDG
---

You will need:

* A PS3 with a DEX firmware (or REX firmware set to DEX mode)

* ProDG Target Manager and ProDG Debugger

* A [debug EBOOT](https://www.reddit.com/r/ps3homebrew/wiki/eboots) of your game

* A wired connection to your PS3 (or place your PS3 in the DMZ of your network for wireless)

1. Start ProDG Target Manager and go to "Search For Targets" and press the refresh button to start scanning. Your PS3 should be detected.

2. Right click your PS3 and move it to the "Debugging Station" group and double click on it. It will add your PS3 into your targets list.

3. In your targets list, right click on your PS3 and choose "Connect". Once your PS3 is connected, you can start ProDG Debugger. If it prompts you to select a target, select your PS3. You will see a window called "Memory", that’s in this window that you will edit the memory of the game you want.

4. Place the debug EBOOT.BIN of your game into the USRDIR directory of your game. It is recommended to keep the original EBOOT.BIN as a backup.

5. In ProDG Debugger you should see a process appear in the "Processes" window, right click on it then choose "Attach Process" and then "Continue without symbols". You can now view memory. By default, when you attach to a process, it will pause the process. To unpause it, go in ProDG Target Manager, expand the list of your PS3, go to "Kernel Explorer", highlight the process then press the "Continue" icon (you can also continue it with ProDG Debugger).

* Like other debuggers, you can add breakpoints, show disassembly, etc. By default, it will only refresh the values when you press the refresh button, but you can also enable "Auto Update" option to have live feeds of the variables.


CID Stealer Protection
---

If you are planning on using a mod tool on your PC in conjunction with TMAPI, it's a good idea to block the program's Internet access so it can't steal your ConsoleID (CID) and upload it to someone else if it is malicious. You can do this with the following process on Windows:

1. Click on your Start Menu and type "Windows Firewall" and select the option that pops up.

2. Select Advanced Settings → Outbound Rules (left side) → New Rule (right side).

3. Follow the wizard and select the .exe file of your mod tool and block it from Domain, Public, and Private networks.