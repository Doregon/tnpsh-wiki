# bguerville toolset

The bguerville toolset provides useful functionality to get information about your console and, more importantly, help you patch your console without factory service mode or a firmware flasher. This option is safer than the ps3xploit default option because of how bguerville’s toolset can verify whether or not the system is downgradeable and prevents you from doing anything without proper initialization of this process.

![](../../.gitbook/assets/bguerville.png)

The bguerville toolset is fairly easy to use and provides tools to patch your firmware and peek/poke your memory at will. It also shows information about your console and can make informed decisions based on that--such as disabling certain features if you have a minimum downgrade praxis of 3.56 or higher, or not letting you use any of the features if you aren't on a PlayStation in the first place. The bguerville toolset is based off of "ps3xploit version 4.0", which was a new exploit found and mastered by bguerville and adapted for this purpose with the toolset.

## Materials Needed

* Internet connection
* A CFW compatible PS3
* Adobe Flash enabled \(the dialog box that asks "Do you want to run the plugin?", make sure you choose yes.\)
* Firmware 4.80 to 4.87

## Patching your flash

Go to the [bguerville toolset](https://ps3xploit.net/bguerrville) page on your console. Switch to the "Flash Memory Manager" tab. Here you should see an option marked **Flash Memory Patch**. If you don't see it, it means you're probably not CFW compatible and should install [PS3HEN](../ps3hen/)

Clicking on this option with show a dropdown box.

![](../../.gitbook/assets/bguerville-patch-1.png)

* **Load Patch from file** searches any connected USB devices and looks for patch files that can be applied to your system.
* **Load Patch from HTTPS** asks you for a URL to download the patch from, let's say, a self-hosted web server.
* **Download Patch file** downloads a patch made my bguerville.  
* The option marked **Apply loaded patch** will be greyed out until a patch is loaded into the console's memory using on of the options above.

Choose your method of loading the patch into the system's memory. Each method comes with obvious drawbacks, but it's easier and more safe to supply your own.

* **If you chose to download from HTTPS or bguerville**, you'll see the download screen.

The patch will be loaded into the system's memory within a few minutes. If it stalls, check your internet connection and try refreshing the page \(not restarting your console\). If you keep having problems, try using a different preparation method to patch your console's flash memory. As you can see below, the dropdown will now have the **Apply loaded patch** option selectable. Obviously, this is because of how you've just loaded the patch into the system's main memory, and now it's time to push it onto the console's NAND or NOR.

![](../../.gitbook/assets/bguerville-patch-3.png)

Once you click the button to patch your flash memory, you'll be prompted with a dialog telling you that **this action cannot be paused once it begins**. Make sure that you have a good power source and that you don't accidentally trip on your console and unplug it--if you console shuts off in the middle of a process like this, you'll have to go to the [flash recovery](https://github.com/Doregon/tnpsh-wiki/tree/7baea441f0febde5dd40f1ee2bdccc3a527f5f28/diags-and-maintenance/flash-recovery.md) page to repair your console and start the process again. This could take about 10-20 seconds on a console with NAND flash, and about 90-120 on a console with NOR flash.

![](../../.gitbook/assets/bguerville-patch-4.png)

If everything's all good, you should see a dialog saying similar things to what's shown below:

* **ROS0 patch operations completed without errors**
* **ROS1 patch operations completed without errors**
* **Patch applied on ROS bank 0/1: YES**
* **Flash Memory successfully patched**

The other information \(Detected Typed, Sector Count, Offset\) will fluctuate based on your console model, firmware, and \(possibly\) other factors relating to any prior modifications to your flash.

![](../../.gitbook/assets/bguerville-patch-5.png)

