---
description: >-
  The PlayStation Network's restrictions, the system's restrictions, the
  company's restrictions, we mean.
---

# Homebrew and the Restrictions

## **If I choose to, will reverting to official firmware make me safe?**

By properly uninstalling all homebrew, clearing your system logs with PSNpatch, and then installing an OFW, there should be no problem. It's recommended to do a full format of your hard drive to remove any possible leftover homebrew files. You can also install the OFW update twice to overwrite your ROS1 hash, which is essentially a record of the last firmware installed. Be warned that if you played unreleased games and connect to PSN, they may ban you when your trophies sync.

## **Will keeping PSN signed out keep me safe?**

Yes. If you plan on staying offline, you can disable PSN altogether to prevent accidental sign on.

## **Can you get banned for using the Internet while signed out of PSN?**

No. It is perfectly safe to use No-PSN versions of apps and the Web Browser while connected to the Internet. If you plan on staying offline, you can disable PSN altogether to prevent accidental sign on, and still be able to use the Internet.

## **Can you get banned by playing on PSN with an ODE?**

There is always a chance that you may get banned by playing on PSN with unauthorized hardware. However, the chance of getting a ban is exceptionally lower than bans from using CFW. Be warned that playing an unreleased game and then syncing your trophies on PSN may result in a ban.

## **Are games region locked?**

The only region locked games are Joysound Dive \(Japan\) and Persona 4 Arena. It is rumored that Way of the Samurai 3 is region locked on Slim consoles. Online services for games may be region locked regardless of the game's region.

## **Are power supplies region locked?**

You should always check the back of your PS3 for the accepted voltages. However, most PS3s support both 110v and 220v, with the exception of some European CECHC and rare batches of late European slim consoles.

## **What temperatures should my PS3 be at?**

You can check your system temperatures by pressing Start+Select on the XMB or in-game XMB \(if Webman is installed\), or you can check it in Multiman. Your PS3 should fall at or below these temperature ranges:

* Fat: 60-70°C idle / 65-75°C PS3 game / 70-80°C PS2 game
* Slim: 55-65°C idle / 65-70°C PS3 game / 70-75°C PS2 game

If your system is above these temperatures, try replacing your thermal paste and/or changing your fan settings with Webman.

## **Why hasn't &lt;insert game here&gt; been ported to PS3?**

Because of the Cell processor architecture, the PS3 is a strange console to develop for and makes porting code difficult. Often times, an entire re-write is required to port an app to the console. Specifically, an N64 emulator has not been finished because it requires a dynamic recompiling library \(DynaRec\) in order to work which would have to be written from scratch and require a massive amount of effort.

# How can I get on PSN?

If you're using an Optical Drive Emulator (ODE), PSN access isn't something you'll have to worry much about. Just keep in mind that just about every firmware update Sony pushes is trying to block your device, so check your ODE manufacturer's website before updating.

On CFW, you can connect to PSN, but you are risking a ban to your account, console, or both. Tools like [PSNpatch](../big-stinky-brew/utilities/psnpatch/README.md) or [SEN Enabler](sen_enabler) can be used to spoof both your firmware version and Console ID, and to hide evidence of CFW on your system in an attempt to avoid bans. It's recommended to use the PSNpatch plugin to prevent yourself from going on PSN *unless* your CFW is hidden. If you plan on playing offline exclusively, follow the procedure on [this page](https://www.reddit.com/r/ps3homebrew/wiki/np_environment) to block PSN completely. Alternatively, if you have a second hard drive on hand, you can use [dual boot firmware](dualboot-fw/README.md) to go online "safely".

The most common reasons for bans are:

* Running homebrew while on PSN. Using Cobra 7.52 or above will help prevent you executing homebrew apps while on PSN.

* Not running [PSNpatch](psnpatch) or similar software to clear your logs and hide your CFW prior to going PSN

* Not using an [antiban EBOOT](antiban) for games that need one

* Playing unreleased games while offline, and then having the trophies sync on PSN

* Modding in public and being reported by other users

If your console does get banned, you can spoof your console's IDPS/Console ID (CID) to another valid CID to unban yourself. A tutorial for this is found [on this wiki page](unban). You may find Console IDs being given away online, they may work, but often get banned within a day. There are also sites offering to sell them, but most of them are not particularly trustworthy, so be wary. Check [this thread out](https://www.reddit.com/r/ps3homebrew/comments/2pywcr/ps3_private_consoleid_psid_for_sale_unban_your_ps3/) for a vendor that has a good reputation.

 

## **Going on PSN with DEX**
If you have DEX firmware or are in DEX mode on Rebug, you may receive an error when trying to sign in. Make sure you have the proper settings with the below procedure:

1. Navigate to Debug Settings on the Settings Tab in the XMB. Make sure the following settings are correct.
 * NP Environment: "np"
 * Release Check Mode: "Development Mode"
 * Boot Mode: "System Software Mode"
 * Network Settings for Debug select "Single Settings"

2. (If on Rebug) Open Rebug Toolbox and navigate to the "Utilities" tab and go all the way down and on "Change Active PS3ID" select "DEX".

3. Run PSNpatch, holding X after launching it. You can now sign in to PSN.

 
## **"Invalid Credentials" Issue**

If you receive a popup saying that your login credentials are incorrect, but you know that it *is* correct, you may have a license agreement that you need to agree to. To fix this, sign in to PSN on the XMB (not in-game) and you should receive a license agreement prompt.

## \*\*\*\*

