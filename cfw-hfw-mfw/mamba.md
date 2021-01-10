# Mamba

[MAMBA/PRX Loader](http://store.brewology.com/ahomebrew.php?brewid=287) is a homebrew that allows you to load MAMBA and/or VSH plugins (with MAMBA or PRX Loader). Mamba features include:

* Region free BluRay
* ISO mounting for BluRay/DVD/PSP/PS1/PS2/PS3
* Mounting ISOs and games over network
* ISOs can be split and still mounted, to bypass FAT32 4GB file limit on USB
* PS1 backup discs work just like retail discs
* Launch any PSP ISO (compatibility is not 100%)
* Launch PS2 ISOs on *any* console (HDD only, software emulator is not 100% compatible)
* Never requires a real disc in drive
* Boot Plugins (apps that run in the background on boot)
* Dynamic firmware spoofing for mounted backups (apps don't require updates for every firmware update)

**Note that Mamba is an alternative to [Cobra](https://www.reddit.com/r/ps3homebrew/wiki/cobra), and therefore incompatible**

## Installation

1. Install MAMBA/PRX Loader PKG

2. Launch "MAMBA/PRX Loader". It will load MAMBA and VSH plugins, and kick you back to the XMB. A single beep indicates no errors. If it beeps more than once, use a [FTP](https://www.reddit.com/r/ps3homebrew/wiki/transferring_files) session to view the log at /dev_hdd/tmp/MAMBA_PRX_Loader.log.

* If you want to load only MAMBA and no VSH plugins hold L1 when MAMBA/PRX Loader starts. 

* If you want to load only VSH plugins and no MAMBA (PRX Loader will be used) hold R1 when "MAMBA/PRX Loader" start. 

Installing the AutoLoader
---

1. Install MAMBA/PRX Loader PKG

2. Launch "MAMBA/PRX Loader" and immediately:
    - Hold CROSS to install "MAMBA/PRX Autoloader"
    - Hold SQUARE to uninstall "MAMBA/PRX Autoloader" 

    A single beep indicates no errors. If it beeps more than once, use a [FTP](../big-stinky-brew/pc-tools/ftp-client.md) session to download and view the log at /dev_hdd/tmp/MAMBA_PRX_Loader.log.

# Boot Flags

Boot flags can be set by creating a file with a specific name in /dev_usb00#/core_flags/ or /dev_hdd0/tmp/core_flags/

- "failsafe" Start in normal mode (MAMBA and VSH plugins are not loaded) 
- "mamba_off" Don't load MAMBA (PRX Loader will be used instead of MAMBA to load VSH plugins) 
- "noplugins" Don't load VSH plugins at boot 
- "verbose" Enable log and write it in /dev_usb00#/ or /dev_hdd0/