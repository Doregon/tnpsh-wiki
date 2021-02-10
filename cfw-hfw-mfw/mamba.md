# Mamba

## Mamba

[MAMBA/PRX Loader](http://store.brewology.com/ahomebrew.php?brewid=287) is a homebrew that allows you to load MAMBA and/or VSH plugins \(with MAMBA or PRX Loader\). Mamba features include:

* Region free Blu-Ray
* ISO mounting for Blu-Ray/DVD/PSP/PS1/PS2/PS3
* Mounting ISOs and games over network
* ISOs can be split and still mounted, to bypass FAT32 4GB file limit on USB
* PS1 backup discs work just like retail discs
* Launch any PSP ISO \(compatibility is not 100%\)
* Launch PS2 ISOs on _any_ console \(HDD only, software emulator is not 100% compatible\)
* Never requires a real disc in drive
* Boot Plugins \(apps that run in the background on boot\)
* Dynamic firmware spoofing for mounted backups \(apps don't require updates for every firmware update\)

**Note that Mamba is an alternative to** [**Cobra**](https://www.reddit.com/r/ps3homebrew/wiki/cobra)**, and therefore incompatible**

### Installation

1. Install MAMBA/PRX Loader PKG
2. Launch "MAMBA/PRX Loader". It will load MAMBA and VSH plugins, and kick you back to the XMB. A single beep indicates no errors. If it beeps more than once, use a [FTP](https://www.reddit.com/r/ps3homebrew/wiki/transferring_files) session to view the log at /dev\_hdd/tmp/MAMBA\_PRX\_Loader.log.
3. If you want to load only MAMBA and no VSH plugins hold L1 when MAMBA/PRX Loader starts.
4. If you want to load only VSH plugins and no MAMBA \(PRX Loader will be used\) hold R1 when "MAMBA/PRX Loader" start.

### Installing the AutoLoader

1. Install MAMBA/PRX Loader PKG
2. Launch "MAMBA/PRX Loader" and immediately:
   * Hold CROSS to install "MAMBA/PRX AutoLoader"
   * Hold SQUARE to uninstall "MAMBA/PRX AutoLoader"

     A single beep indicates no errors. If it beeps more than once, use a [FTP](../big-stinky-brew/pc-tools/ftp-client.md) session to download and view the log at /dev\_hdd/tmp/MAMBA\_PRX\_Loader.log.

## Boot Flags

Boot flags can be set by creating a file with a specific name in /dev\_usb00\#/core\_flags/ or /dev\_hdd0/tmp/core\_flags/

* "failsafe" Start in normal mode \(MAMBA and VSH plugins are not loaded\) 
* "mamba\_off" Don't load MAMBA \(PRX Loader will be used instead of MAMBA to load VSH plugins\) 
* "noplugins" Don't load VSH plugins at boot 
* "verbose" Enable log and write it in /dev\_usb00\#/ or /dev\_hdd0/

