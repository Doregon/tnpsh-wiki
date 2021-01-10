# Exploiting your Console using HAN

**Note that this method is obsolete due to PS3HEN, and is not supported on firmwares greater than 4.84.** 

PS3Xploit 3.0 "etHANol", shortened to "HAN", is an addition to PS3Xploit which allows the installation of PKG files on OFW. While it cannot be used to install homebrew PKGs, it can be used to install PS3, PS2, PS1, and PSP game backups. HAN is currently only stably supported on 4.84 HFW.

A video demonstration of installing HAN can be found [on MrMario2011's channel](https://youtu.be/xItN2trbaSY?list=PL1CadovfabPsSL6j1QRMJrThmnZFaNMe6).


## Materials Needed

* A USB storage device, **formatted as FAT32 with 32kb allocation size**

* [HAN support files](http://ps3xploit.com/files/release/han_supportfiles.zip) (extracted on your desktop)

* [4.84 HFW .PUP](https://mega.nz/#!zQQwXIIB!8KKPcY34Qjh-l9ZkYLax68FfuWM9D1VGFl26mD_NKk8)

## (Method 1) Using an Exploit-Loading Site

This method uses online-hosted sites for loading HAN onto your system. While there are other sites out there, PS3Xploit.com is the official site for HAN. **Ensure that you are on 4.84 HFW**.

1. Update to 4.84 HFW using [this guide](https://www.reddit.com/r/ps3homebrew/wiki/installing_cfw) and the .PUP linked in the "Materials Needed" section.
 - [Verify the MD5 checksum](https://reddit.com/r/ps3homebrew/wiki/md5) of the PUP matches the checksum:  `4247362B54FADD2E4D7C09007F720803` before continuing. If they match, you may continue, otherwise you will need to redownload the PUP and verify again.

2. Navigate to the first column (called Users) in the XMB and create a new user. This user is going to be your main HAN user account, where you will be doing most of your HAN activity in

3. After making the new user, log in to it and navigate to the far right column and create a new PSN account. If you do not wish to use a real email address, you can use [temp-mail.org](https://temp-mail.org) to create it.

4. When you've successfully made the PSN account and have logged onto it, navigate back to the PSN column, click Account Management and click activate. It will ask you what you want to activate, at which point you should select Game and continue.

5. Sign out of the PSN account and restart the console.

6. Go to your computer and ensure that your USB drive is formatted as FAT32 with 32kb allocation size, and check that the USB drive is recognized by your PS3 and shows up on the XMB under the Photos, Music, or Videos columns. Extract the files from han_supportfiles.zip onto the root of your USB drive. Also, copy the HAN Toolbox PKG onto the root of your USB drive.

7. Plug the USB drive in the **right-most** USB port of the PS3.

8. Login to the HAN account you just created, then open the Internet browser and navigate to ps3xploit.com. You will be presented with a white menu at the top of the screen. On that menu, hover over "v3 HAN Tools" to expand a sub-menu from which you will press Cross to select "HAN installer".

9. PS3Xploit will notify you that you are capable of installing HAN, press Cross to dismiss the message and you will be presented with a yellow page that says "PS3 HAN installer".

10. Press Triangle on your controller, navigate over to Tools, then select "Home page" > "Use Current" and press Cross to accept.

11. Exit out of the browser and open it again. You will be presented by the same yellow page.

12. Select "Initialize HAN installer", wait for it to initialize, then select "Launch HAN installation" when the option becomes available.

13. If your PS3 restarted, you've successfully installed HAN. If for some reason your PS3 didn't restart or you got an error, you need to start over.

14. Ensure that you are on logged into your HAN profile. 

15. Open the browser and navigate to ps3xploit.com again. On the white menu at the top of the screen, hover over "v3 HAN Tools" and select "HAN Enabler". You will be presented with a yellow page, labelled "PS3 HAN Enabler".

16. Press Triangle on your controller, navigate to Tools, then select "Home page" > "Use Current" and click OK.

17. Close the browser and open it again.

18. Select "Initialize HAN Enabler", wait for it to initialize, then select "Enable HAN" once that option becomes available. 

19. The browser will ask you if you want to close it, choose "Yes" and you will be returned to the XMB.

20. Navigate to the Games column on the XMB, select Package Manager, then select Install Package Files > Standard. The HAN Toolbox PKG should be there. Press Cross on it to install the HAN Toolbox.
 * If you ever wish to uninstall HAN Toolbox, navigate to Game Data, hover over HAN Toolbox icon, press Triangle, and Delete.