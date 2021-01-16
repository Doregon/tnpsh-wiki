# Dealing with 4GB+ Files

PS3 games will occasionally have files >4GB which, due to the limitations of FAT32, can cause problems if you are planning on using it on an external hard drive or transferring it to a flash drive. Fortunately, there are a number of solutions to this problem.


# Internal Drive

The filesystem on the PS3's internal drive does not have this limitation. You can FTP large files to and from the drive without any problems. Most backup managers have built in FTP servers to make this easier. multiMAN can also join split files back together if you use the Split Files method below.

# NTFS (external)

Hard drives in NTFS format will not have the 4GB limitation. However, they have a few limitations. More information can be found [here](https://www.reddit.com/r/ps3homebrew/wiki/ntfs).

# Zipping Files

One option to move 4GB+ files to your PS3 is to use a tool such as 7zip or WinRAR to zip a 4GB+ file. If your zipped archive is less than 4GB, you can transfer it to your internal hard drive and unzip it [using multiMAN's file manager](../big-stinky-brew/file-managers/multiman/README.md). Note that this only supports .ZIP extensions; .RAR or .7z will not work. 

# Extract ISO

if you are dealing with a single large PS3 or PS2 ISO, you can try extracting using a tool such as WinRAR or 7zip. If it's a PS3 game, you can place it it in a folder of any name inside of your GAMES folder on your internal hard drive, or GAMEZ folder on an external FAT32 hard drive. If you want to convert it back to a single ISO, or if you have an extracted PS2 ISO, you must use multiMAN's file manager to select the folder containing the extracted files, press Circle → Cut, and then Circle → "Paste as ISO" to recombine it to an ISO. Make sure to put the resulting ISO into PS2ISO or PS3ISO.

# Split ISO

Using [Cobra](../cfw-hfw-mfw/cobra.md) or [Mamba](../cfw-hfw-mfw/mamba), ISO files can be split in half and still played. You can use the PS3 File Splitter program bundled in [Aldostools](../big-stinky-brew/aldostools-collection/README.md), which will scan through a folder or file and split any big files into files of the specified size. You can choose the extension for the split files, all of which should work (recommended is .\#\# for simplicity).

Alternatively, you can use [PS3 ISO Tools](http://psx-scene.com/forums/f6/article-ps3-iso-tools-updated-version-2-0-a-125145/index3.html#post1152989) by selecting the "Split ISO(s)" option and the CFW and "Firmware 4.66" settings (regardless of your actual firmware version).


# Split Files (PSARC)

You can use multiMAN's file manager to rejoin split files. Browse to the first split file and press Circle on the first split file (.#, .psarc#, or .666##) file → Cut, browse to another folder and press circle → Paste. It will automatically copy and combine all of the other split files into one file. Press circle → Cut on the new file, and paste it back in the original directory. This may not work with all files, so you may need to transfer the split files to your PC, combine them with PS3 File Splitter (in Aldostools), and FTP the merged file back.