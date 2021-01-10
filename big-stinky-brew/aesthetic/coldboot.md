# Custom Coldboots and PSN Logo

**WARNING: The tutorials on this page involve modifying files in the flash. There is a potential for something to go wrong and being unable to start up your PS3 properly. This can be fixed by re-installing your CFW.**

What is a coldboot? A coldboot consists of the logo and sound played when your console is booting up. The unmodified version displays "PS3" and plays an orchestra sound effect. With modifications, you can use [any images](http://oi39.tinypic.com/2uyhj7c.jpg) that you want, with any sound up to 8 seconds long. 

**NOTE: Do not install coldboots that were not designed for your firmware version. This may result in a brick and require you to reinstall your firmware.**

## Coldboot Collection ISO

A collection of coldboot logos are available on the [XMB Mods Collection ISO](http://store.brewology.com/ahomebrew.php?brewid=303) (or on the smaller [PS3 Coldboots Collection ISO](http://www.mediafire.com/download/ew50hhj6ftc8ec3/Coldboots+collection+disc.iso)). You can apply the coldboots as follows:

1. Download and [transfer](https://www.reddit.com/r/ps3homebrew/wiki/transferring_files) the ISO file to /dev_hdd0/PS3ISO/.
2. Mount the ISO using a backup manager such as Multiman or Webman.
3. Select the disk, and choose the desired coldboot.
4. Press Cross to install and Yes when prompted. You will be returned to the XMB. 
5. Reboot to verify that it works.


## Creating a Coldboot Logo with RAF Converter

You will need the following:

- The completed image you wish to use in place of the PS3 logo

- [Easy Static RAF Converter](http://www.mediafire.com/download/7rnjy5n2ki6u6z3/Easy+Static+RAF+Converter+v1.0a.exe)

1. Open Easy Static RAF Converter and select your image. Any resolution image will work, although it will crop the image to what you see in the preview window.
2. Click "Show Preview" and drag the window off to the side so that you can see both windows simultaneously.
3. Change the height and width to the size you want; the default custom values are the natural size of the image. An easy way to keep the same size ratio is to use a [calculator](http://www.csgnetwork.com/pixelratiocalc.html) and plug in the original numbers, then a custom number for the desired height/width.
4. Choose a position or coordinates for the image. The X coordinate can be a negative or positive value (max 1920) from left to right and the Y coordinate can be a negative or positive value (max 1080) top to bottom.
5. Select the Convert button; the program may freeze or hang, just click OK and wait for it to say "Done".
6. Your newly generated coldboot.raf file will be in a folder named the same as your original image.
7. Apply the Coldboot logo using the "Applying the Coldboot or Logo" section below.

## Creating a Coldboot Logo with Photoshop

You will need the following:

- Adobe Photoshop

- [Adobe DDS Plugin](http://developer.nvidia.com/object/photoshop_dds_plugins.html)

- [PS3 Boot Logo Creator](http://ps3.brewology.com/downloads/download.php?id=12574&mcid=4)

1. Install the DDS Plugin.
2. Open a DDS file in the "Boot Logos" folder and choose "Load using Default Size".
3. Edit the image as desired, but **do not change the size of the image**.
4. Save the image; when prompted, use the settings "8L 8pp | luminance", 2D Texture, and Generate MIP maps.
5. Repeat steps 2-4 the process for all 6 images, making sure not to resize the images.
6. Run "Coldboot Creator.exe" and choose the option under "Step 1".
7. Click "Convert Pictures" and follow the instructions to convert your DDS files into GTF files.
8. Click Browse on each row and select the GTF versions of the files and press Start.
9. Click the option under "Step 2" and follow the instructions.
10. Click the option under "Step 3" and follow the instructions.
11. Browse to the files it asks for and click finish to generate the final Coldboot.raf file.
12. Apply the Coldboot logo using the "Applying the Coldboot or Logo" section below.

## Creating Coldboot Audio

1. Download and install [XviD4PSP](http://www.videohelp.com/software/XviD4PSP).
2. Create the sound you want; it can be any normal format as long as it is shorter than 8 seconds long. You can edit and trim files within XviD4PSP if you don't have a sound editor.
3. Open the file in XviD4PSP.
4. Change the settings to:

> Format: Audio

> Filtering: Disabled

> Color Correction: Disabled

> Video Encoding: Disabled

> Audio Encoding: A3C 640K Quality

5. Click "Encode" and save it with the filename "coldboot_stereo.ac3".
6. Click "Encode" again and save it with the filename "coldboot_multi.ac3".
7. Apply the Coldboot audio using the "Applying the Coldboot or Logo" section below.


## Applying the Coldboot

1. Enable writing to flash on your PS3. This can be done with a pkg file for your specific CFW, or enabled in Rebug Toolbox for Rebug systems.
2. [FTP](https://www.reddit.com/r/ps3homebrew/wiki/transferring_files) into your PS3 and browse to /dev_flash/. This directory may be called /dev_blind/ or /dev_rebug/ depending on your system. It does not always appear even if you enabled writing to flash, so try manually typing in the directory name to get to it.
3. Download the file(s) you will be replacing to your PC (coldboot.raf, coldboot_stereo.ac3, coldboot_multi.ac3, and/or xmb_plugin_normal.rco) and keep them in a safe place in case something looks wrong and you want to revert back.
4. Copy the coldboot.raf, coldboot_stereo.ac3, coldboot_multi.ac3, and/or xmb_plugin_normal.rco file(s) you generated to /dev_flash/vsh/resource.
5. Reboot and enjoy your new mods! It is suggested to disable writing to flash on your PS3 to prevent corruption on reboots.

* If your console does not boot properly, boot your console into [recovery mode](http://community.us.playstation.com/t5/PlayStation-3-Support/How-to-access-the-PlayStation-3-Recovery-Menu/td-p/19195118) and [re-install your firmware](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw)


Troubleshooting
---

If your console has strange issues, such as hanging when launching apps, reinstall your firmware to reset it to a working state.