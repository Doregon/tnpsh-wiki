# CEX and DEX

## Converting Between CEX and DEX

Early in the PS3 scene, specific mods and tweaks were only possible on DEX firmware. Nowadays, DEX features are often possible on CEX firmwares and DEX custom firmwares are becoming a thing of the past. The following instructions will show you how to convert your PS3 to either CEX or DEX.

A video demonstration of converting your console to DEX can be found on [MrMario2011's channel](https://youtu.be/tmpexUf9eK0?list=PL1CadovfabPsSL6j1QRMJrThmnZFaNMe6).

* Note that if you plan on going online, you will need to change some options in Debug Settings to enable online. You can find how to do this [here](https://www.reddit.com/r/ps3homebrew/wiki/psn#wiki_going_online_with_dex).

## Swapping Between CEX and DEX

1. Install the latest Rebug firmware from Rebug.me if not already installed. A tutorial to do this can be found [here](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw). Choose REX firmware if you are currently on CEX, and D-REX firmware if you are currently on DEX.
2. Once you're at the XMB, install Rebug Toolbox and open it. You can find it under Install Packages → System.
3. Go to the utilities column \(far right\) and select Toggle QA Flag. Select "Enable". Your console should beep and return to the XMB.
4. From the XMB, go back into Rebug Toolbox and navigate to utilities column \(far right\) and select "Dump eid\_root\_key".
5. On this screen select "Yes". The screen will go blank and after 10 seconds you will hear 3 beeps and the system will re-boot.
6. Go back into Rebug Toolbox and go to the "DEX & CEX" column \(second from the right\) and select "Rewrite target ID in flash" and select "Yes". Your console with either reboot or show turn black momentarily. If your console did not reboot, browse up one setting and select "Swap LV2 Kernel" and select "Yes". Your console will reboot.
7. Verify the system type you are on by entering Rebug Toolbox, browsing to the far left, and selecting System Information. You are now free to install any other CFW or stay on Rebug \(recommended\).
   * If your system freezes a bit after rebooting, make sure to turn the "What's New?" option off under Settings → "Display \[What's New\]" → Off, and reboot.

