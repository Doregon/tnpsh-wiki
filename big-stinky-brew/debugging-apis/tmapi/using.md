# Preparing your PS3

* Start ProDG Target Manager and go to "Search For Targets" and press the refresh button to start scanning. Your PS3 should be detected.
* Right click your PS3 and move it to the "Debugging Station" group and double click on it. It will add your PS3 into your targets list.
* In your targets list, right click on your PS3 and choose "Connect". Once your PS3 is connected, you can start ProDG Debugger. If it prompts you to select a target, select your PS3. You will see a window called "Memory", that’s in this window that you will edit the memory of the game you want.
* Place the debug EBOOT.BIN of your game into the USRDIR directory of your game. It is recommended to keep the original EBOOT.BIN as a backup.
* In ProDG Debugger you should see a process appear in the "Processes" window, right click on it then choose "Attach Process" and then "Continue without symbols". You can now view memory. By default, when you attach to a process, it will pause the process. To unpause it, go in ProDG Target Manager, expand the list of your PS3, go to "Kernel Explorer", highlight the process then press the "Continue" icon \(you can also continue it with ProDG Debugger\).
* Like other debuggers, you can add breakpoints, show disassembly, etc. By default, it will only refresh the values when you press the refresh button, but you can also enable "Auto Update" option to have live feeds of the variables.

