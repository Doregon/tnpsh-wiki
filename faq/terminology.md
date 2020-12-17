---
description: Need to know the difference between CFW/HFW/OFW/MFW?
---

# Terminology

## **What do the letters mean in a Title ID?**

That information can be found here.

## Definitions of common terminology

| Term | Definition |
| :---: | :---: |
| **Custom Firmware \(CFW\)** | Firmware modified to add in extra features not present in original firmware \(OFW\). |
| **Original Firmware \(OFW\)** | Stock firmware released by Sony. |
| **Hybrid Firmware \(HFW\)** | Hybrid firmware released by the PS3Xploit team to include the WebKit version that was used in 4.82 in newer firmware packages, making exploitation of newer firmwares possible. |
| **Modified Firmware \(MFW\)** | Personal custom firmware created using the MFW Builder. They provide an open framework for mods and plugins on the system and the running of unsigned code. It is recommended to stay away from MFW unless it is from a trusted source or yourself. |
| **Consumer Firmware \(CEX\)** | Retail system firmware; consumers like yourself buy CEX consoles in stores. |
| **Developer Firmware \(DEX\)** | Debug system firmware; game developers use DEX consoles for making and testing games. In the past, you could only mod games on DEX firmware, but now it is possible on CEX as well. The only real benefit of using DEX is for legacy modding tools, connecting to developer PSN \(sp-int\) if Sony whitelists you, and certain features of [PS3XPAD](https://www.reddit.com/r/ps3homebrew/wiki/ps3xpad). |
| **Rebug Firmware \(REX\)** | Rebug-only firmware that must be installed over CEX firmware and allows swapping between CEX and DEX kernels. |
| **Rebug Firmware \(D-REX\)** | Rebug-only firmware that must be installed over DEX firmware, otherwise identical to REX. |
| **Store Firmware \(SEX\)** | Shop/demo firmware used for store displays. In order to convert back to CEX, you must install a "kiosk reverter" firmware update. It is a limited version of CEX. |
| **Arcade Firmware \(GEX\)** | Firmware for [arcade systems](http://www.psdevwiki.com/ps3/Template:Arcade_models); similar to SEX firmware, it has no purpose outside of being used in arcades. Under NO circumstances should you install GEX firmware, there are no known ways of reverting it back. |
| **Tool Firmware \(DECR\)** | Firmware for [DECR stations](http://www.gamesniped.com/wp-content/uploads/2013/01/Sony-Playstation-3-Reference-Tool-DECR-1000A-SY5.jpg); only meant to be run on old DECR development stations which emulate various PS3 models for testing. Under NO circumstances should you attempt to install it on a PS3. |
| **CID** | A console ID \(CID\) is a community coined term to describe a PSID and IDPS together when bought or sold. They are used to unban consoles. Private CIDs are ones that have never been shared with anyone, and public CIDs are ones posted publicly and are prone to a quick banning. |
| **CECH** | The start of PS3 model numbers, followed either by a single letter \(for fat consoles\) or by a four digit number \(for slim and super slim consoles\). |
| **EDAT** | Encrypted data. This is data for a game or DLC which is often licensing information that locks C00 games or demos that contain the full game. LIC.EDAT is an old licensing system to use games made circa 2010 and earlier. |
| **EE** | Emotion Engine chip. The PS2 CPU, which is found in early fat consoles. |
| **GS** | Graphics Synthesizer chip. The PS2 GPU, which is found in early fat consoles. |
| **HDCP** | High Bandwidth Digital Content Protection. A digital copy protection which prevents recording of the HDMI signal. Some capture cards and HDMI splitters can overcome this. |
| **CELL BE** | CELL Broadband Engine chip. The PS3 CPU. |
| **RSX** | Reality Synthesizer chip. The PS3 GPU. |
| **IDPS** | A 32-character unique fingerprint for online tasks such as checking if your console is on the banned console list. This can be spoofed to another legitimate IDPS. |
| **Internet Relay Chat \(IRC\)** | A popular form of real-time Internet text messaging \(chat\) or synchronous conferencing. It is mainly designed for group communication in discussion forums, called channels, but also allows one-to-one communication via private message as well as chat and data transfer \(including file sharing\). |
| **Metldr/Metldr2** | Metldr was the hardware-buried lowest level private encryption key that was figured out and made signing CFW possible. It was replaced with metldr2 in firmwares after 3.55, and in hardware starting around April, 2011 \(datecode 1B\). |
| **Peek / Poke** | Peek is the generic term for a system call that lets you read a memory address. Poke is the the term for a syscall that lets you write to any memory address. They are required for backup managers to work properly. A userspace application can use these syscalls to dump out the entire memory space of the kernel, or patch the kernel as it is running. |
| **PKG** | An installation file that can be run from the XMB to install software on the PS3. |
| **PSID** | A 32-character unique fingerprint for offline tasks such as linking your console to HDD backups and game saves. This can be spoofed to another PSID. |
| **RAP** | RAP files are a file used in conjunction with your PS3 and ReactPSN/PSNpatch to make RIF \(license\) files for games. |
| **RIF** | RIF files are licenses specific to your PS3 that allow your user profile to play a PSN game or DLC. |
| **RLOD/YLOD** | Red Light Of Death or Yellow Light of Death. Caused by hardware malfunction, often due to overheating. |
| **RSOD** | Red Screen Of Death. Caused by software/firmware malfunction. Usually requires a reinstallation of firmware. |
| **ROS0/ROS1** | Checksums of your currently installed and last installed firmware. Installing a firmware will change whether ROS0 or ROS1 is active, and corruption in the inactive ROS is OK. |
| **SEN / PSN** | Sony Entertainment Network, also known as the PlayStation Network \(PSN\) is the online PlayStation service. |
| **Syscall** | An operating system function. There is a limited number of these which can be called from an application or game. Extra syscalls are added with CFW to allow extra functionality, but access to these syscalls can be detected when on PSN. |
| **Signing** | The process of setting a PKG file such that it appears to the PS3 as a normal, officially allowed package. All PSN games, updates, etc. are signed, and must be so for the PS3 to allow them to install. |
| **XMB** | Xross Media Bar - Graphical Interface User designed as a cross. Used on the OS on PSX, PSP, and PS3 and other Sony Products. |
| **nm** | Nanometer. |

