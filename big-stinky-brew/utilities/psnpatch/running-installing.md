# Running PSNpatch

## Running PSNpatch Manually

1. If planning on playing a game backup online, mount the game first.
2. Launch PSNpatch and continue holding Cross until you hear a beep, indicating that the CFW Syscalls have been disabled, execution history cleared, and IDPS spoofed \(if one is set in the config file\). If you do not hear a beep, it has not completed successfully.
3. It is highly recommended to install the Safety Plugin to prevent connecting to PSN without first running PSNpatch.

## Installing the Safety Plugin

**THE SAFETY PLUGIN DOES NOT WORK ON DEX FIRMWARE**. Some people have also reported boot issues with the plugin on 4.82 firmwares. The safety plugin will prevent you from connecting to PSN unless you have run PSNpatch or used a button combo to run it.

1. Launch PSNpatch and enter the TOOLBOX sub-menu by pressing the ENTER button as shown on your screen.
2. Follow the on-screen instructions to enable the plugin and reboot. Your console will now have PSN disabled at boot-up.
3. Press L3+R3+R2; CFW will be disabled, IDPS spoofed, game execution history cleared, and PSN connection unlocked. You can now sign into PSN.
   * If it freezes after a reboot, try holding `SELECT + L2 + R3 + L3` on bootup to remove your boot\_plugins.txt file and prevent the plugin from booting up

