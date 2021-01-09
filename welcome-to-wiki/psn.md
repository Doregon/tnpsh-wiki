# How can I get on PSN?

If you're using an Optical Drive Emulator (ODE), PSN access isn't something you'll have to worry much about. Just keep in mind that just about every firmware update Sony pushes is trying to block your device, so check your ODE manufacturer's website before updating.

On CFW, you can connect to PSN, but you are risking a ban to your account, console, or both. Tools like [PSNpatch](/big-stinky-brew/utilities/psnpatch/README.md) or [SEN Enabler](sen_enabler) can be used to spoof both your firmware version and Console ID, and to hide evidence of CFW on your system in an attempt to avoid bans. It's recommended to use the PSNpatch plugin to prevent yourself from going on PSN *unless* your CFW is hidden. If you plan on playing offline exclusively, follow the procedure on [this page](https://www.reddit.com/r/ps3homebrew/wiki/np_environment) to block PSN completely. Alternatively, if you have a second hard drive on hand, you can use [dual boot firmware](dualboot-fw/README.md) to go online "safely".

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