# Custom SND0.AT3

Sony games use a proprietary audio codec called ATRAC3 \(.AT3\) which is used for game sounds on the XMB and [coldboots](https://www.reddit.com/r/ps3homebrew/wiki/coldboots). It is possible to create your own songs or audio clips to play when viewing apps in the XMB or when your system boots up. This guide will cover creating custom ATRAC3 files to replace in your backup games or homebrew. This process works on both PSP and PS3 games.

## Required Items

* [GoldWave version 5.10](https://mega.nz/#!97YzlLga!XkQ1O3hJjxedfGFyGkpLK2r964CznWfTLKYPTwHIPQo)
* [ATRAC3 Codec](https://mega.nz/#!1rgFwZLY!SkuMOcqepMV2OJNQV_XuVn0GOJ-nu3uoTZE8XWMGe0s)
* [GoldWave AT3 Looping Tool \(GWAT3\)](https://mega.nz/#!g2Ry0SKb!m-epOH2GY7NVXwCfza_IiSDLX7IlIpn6NdqkoI7vyg0) 

## Creating the SND0.AT3 Files

1. Install GoldWave 5.10. 2. Install ATRAC3 Codec. If you are on a 64bit version of Windows or Windows 7 and later follow the next step.

```text
    Installing 32bit Codecs on a 64bit machine:

    1. Copy the extracted .acm file into \Windows\SysWOW64\ 
    2. Create a new notepad file and paste the following:

    Windows Registry Editor Version 5.00

    [HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32]
    "msacm.atrac3acm"="atrac3.acm"

    [HKEY_LOCAL_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\drivers.desc]
    "atrac3.acm"="Sony ATRAC3 ACM"


    3. Save as 'atrac3.reg' and place it in \Windows\SysWOW64\ 
    4. Run the 'atrac3.reg' file, Windows should accept the registry edit. Restart your computer.
```

3. Open GoldWave and open a MP3 you wish to use. You must use the trim function in GoldWave to trim the audio down to around 50-55 seconds, or 8 seconds maximum for a coldboot. Anything longer will likely not work. The Fade Out tool is optional to make it sound better when played.

4. Go to EFFECT in the toolbar and choose 'Playback Rate'. Assuming your mp3 is a generic 44100Hz, you will need to change the sample rate to 40200Hz. The PS3 uses the sample rate of 48000Hz, so to make your MP3 sound normal when played via the XMB you need to drop the sample rate by the difference of your song and the PS3 sample rate \(3900Hz\).

* For PSP, do not change the sample rate

5. File → Save As.

* Save as Type: Wave \(\*.wav\)  
* Attributes: ATRAC3 132kbps STEREO  
* For PSP, use 66kbps instead

You may get a pop up window warning about the sampling rate, just close it. When saving your file you may get a pop up asking to update the sound window with the new format, choose No.

The file saved is now a .wav. You will need to manually change the file type to .AT3. See [here](https://support.microsoft.com/en-us/help/865219/how-to-show-or-hide-file-name-extensions-in-windows-explorer) to enable file extensions in Windows.

6. This step is optional: Looping your newly created ATRAC3 file.

* Open GWAT3 and select your AT3 file and click Start.  
* GWAT3 will create a looped copy of your song.AT3 in its directory.  

7. Navigate to the root of your PS3 game/homebrew folder and replace the file SND0.AT3. Your new file must be named SND0.AT3 as well.

8. Load up your game or homebrew in XMB, or your apply your coldboot, and you should hear your song play.

