# About Jailbreaking

## **What is the point of jailbreaking?**

The intent of jailbreaking was to allow execution of homebrew software on the PS3. Custom firmware will allow you to:

* Play backups of PS3 / PS2 / PSX / PSP / Blu-Rays / DVDs natively and region free, even on non-backwards compatible models.
* Emulate retro games with RetroArch or stand-alone emulators.
* Rip PS3 / PS2 / PSX / Blu-Ray / DVD discs to your hard drive.
* Rip Super Audio CD \(SACD\) discs
* Mod games offline or on PSN.
* Convert your console to developer firmware \(DEX\).
* Play games stored on an external drive, or even one stored elsewhere on your network.
* Use a NTFS hard drive to get past 4GB file limitations and have unlimited storage capacity.
* Unban your console.
* Change the boot up logo and sound and remove the epilepsy warning for a faster boot up.
* Use Linux.
* Use the console to its full extent with a broken Blu-Ray drive.
* Put a completely new \(same model\) Blu-Ray drive into your console with your motherboard without having to take the drive apart.
* Use custom devices, such as an Xbox 360 gamepad, as controllers with PS3XPAD.
* Install Movian, a Media Center application in which you can download plugins such as TV channels and Torrent Streamers.
* Install homebrew games and apps.

## **Can you jailbreak consoles over 3.55 OFW without downgrading or buying a flasher device?**

Yes, you can use PS3Xploit to install CFW. Prior to Thanksgiving of 2017, it was impossible to downgrade without a flasher device, and you could not jailbreak consoles over 3.55 firmware. Because of this, there are many sites out there claiming to offer PUPs that will jailbreak your console, but any sites claiming to do this without using PS3Xploit are a scam or malware.

## **Do I need to have the latest OFW installed before jailbreaking?**

If you are on or below 3.55, you can go directly to CFW. If you are on firmware above 3.55, you will need to check if your console is exploitable and the requirements therein.

## **What is Hybrid Firmware \(HFW\)?**

A. HFW is a modified version of 4.84 OFW which includes the WebKit version that was used in 4.82 to make the original PS3Xploit, hence the name, "Hybrid Firmware".

## **Do I need to go to 9.99 Downgrader or 3.55 OFW before going to CFW?**

No. It's recommended to go straight to the latest CFW after flashing a patched dump to your PS3 or using PS3Xploit. Sometimes issues crop up and people get stuck on downgrader firmware and are forced to format their hard drive to get off of it. Downgrader firmware was the old method of getting to CFW.

## **Why can't consoles with minimum firmware over 3.56 be jailbroken?**

Essentially, Sony slipped up and their lowest level encryption key \(metldr\) was figured out. They improperly generated their update signature decryption key and a number that was supposed to be random was actually a static number. With this, developers could sign a modified update \(CFW\), which a console on 3.55 or lower will accept as an official update. This was patched in 3.56, but models that were once on 3.55 firmware still have the old key in its hardware, and therefore can be exploited using PS3Xploit or a hardware flasher.

## **Why can't certain consoles be downgraded to 3.55?**

Every console leaves the factory with a "minimum downgrade praxis". It's a long and complicated thing with eFUSES and burning into the CPU, but basically this is a hardcoded number of the lowest possible firmware version the console can handle. Due to all CECH-30XX, Super Slims, and some CECH-25XX's leaving the factory with a minimum downgrade praxis above 3.56, they are unable to be downgraded to 3.55.

## **What about a minimum praxis of 3.56?**

These consoles, usually being a CECH-25XX with datecode 1A, are a special exception. They can be flashed with a flasher device and have a 4.XX CFW installed. The key difference here is that you cannot install 3.55 firmware on it, or else it will be bricked. The reason for this special exception is that, although they came from the factory with 3.56 firmware, they still have old lowest level encryption key \(metldr\) in their hardware.

## **What is the future potential of the scene?**

More emulators, better PS2 game compatibility than OFW, or even a completely new XMB could be developed.

## **What backups are supported?**

Currently you can run PS3, PS2, PSX, and PSP natively on CFW. More emulators can be downloaded to play older systems using RetroArch or stand-alone emulators.

## **I have a jailbroken console. What should I do first?**

See this page for recommendations on what to install first.

## **What firmware should I get?**

That's up to you. Research around and find what's most appealing to you. Check out this page for the names and links to the major firmware brands. The most popular is Rebug due to it supporting both CEX and DEX modes.

## **Is there a reason to use significantly older CFW?**

No. It's best to use the latest CFWs which include the latest features, and the latest stability patches from OFW. It is safer to play on PSN with updated firmware, as firmware updates can change how it connects to PSN.

## **I'm trying to update my firmware via USB, and it says it's missing/corrupted?**

Ensure that the update is named PS3UPDAT.PUP and is placed on a flash drive in the directory "X:\PS3\UPDATE\". If you are attempting to install Rebug, and don't know exactly what firmware you are currently on, try both REX and D-REX versions, as D-REX is the same firmware but allows you to install it over DEX.

## **Are there nightly builds of CFW?**

No. CFW is generally made, tested in public, then released after all models have been tested. All CFW releases should be a "stable" release.

## **What is Cobra/Mamba?**

See this page for information about Cobra, and this page for information about Mamba.

