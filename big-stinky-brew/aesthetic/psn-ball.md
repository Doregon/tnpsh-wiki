# PSN ball

The PSN ball \(or logo\), is the icon on top of the PSN column on the XMB. For more customization, see the [themes page](https://github.com/Doregon/tnpsh-wiki/tree/2fdb48620ab1dcfea983a2949cb04bb755d07cca/big-stinky-brew/aesthetic/themes.md).

Changing PSN Ball / Logo

## PSN Icons ISO Method

A collection of custom PSN Icons are available on the [XMB Mods Collection ISO](http://store.brewology.com/ahomebrew.php?brewid=303) \(or the smaller [PSN Icons Collection ISO](https://www.dropbox.com/s/nt2lr1pqoqmtova/PSN%20icons%20collection%20disc.iso?dl=0)\). You can apply the fonts as follows:

1. Download and [transfer](https://github.com/Doregon/tnpsh-wiki/tree/2fdb48620ab1dcfea983a2949cb04bb755d07cca/big-stinky-brew/pc-tools/ftp-client/README.md) the ISO file to /dev\_hdd0/PS3ISO/.
2. Mount the ISO using a backup manager such as multiMAN or webMAN.
3. Select the disk, and choose the desired icon.
4. Press Cross to install and Yes when prompted. You will be returned to the XMB. 
5. Reboot to verify that it works properly.

## Manual Method

1. Download a PSN ball that you like, various packs can be found on Google.
2. Extract the one you want and make sure it is named as "xmb\_plugin\_normal.rco".
3. Apply the PSN logo using the "Applying the Coldboot or Logo" section below.

## Applying the PSN ball

1. Enable writing to flash on your PS3. This can be done with a pkg file for your specific CFW, or enabled in Rebug Toolbox for Rebug systems.
2. [FTP](../pc-tools/ftp-client.md) into your PS3 and browse to /dev\_flash/. This directory may be called /dev\_blind/ or /dev\_rebug/ depending on your system. It does not always appear even if you enabled writing to flash, so try manually typing in the directory name to get to it.
3. Download the file you will be replacing to your PC \(xmb\_plugin\_normal.rco\) and keep them in a safe place in case something looks wrong and you want to revert back.
4. Copy the xmb\_plugin\_normal.rco file you downloaded or copied to /dev\_flash/vsh/resource.
5. Reboot and enjoy your new mods! It is suggested to disable writing to flash on your PS3 to prevent corruption on reboots.
6. If your console does not boot properly, boot your console into [recovery mode](https://github.com/Doregon/tnpsh-wiki/tree/2fdb48620ab1dcfea983a2949cb04bb755d07cca/diag-and-maintenance/recovery.md) and [re-install your firmware](../../cfw-hfw-mfw/firmware-upgrading.md)

