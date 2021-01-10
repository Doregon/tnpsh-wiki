---
description: Thinking about building or catching up on what's new with the devs?
---

# Developer Information

## **What is the QA Flag?**

The QA Flag is a setting that is enabled when a console is in the Quality Assurance stage before it leaves the factory. It allows access to Debug Settings. It also allows downgrading to a lower version of firmware without use of downgrader firmware. It can be enabled with Rebug Toolbox or the qa\_toggle package, or by enabling HEN.

## **Debug Settings isn't showing up under the Settings column, why?**

A. Your PS3 must have the QA Flag enabled, which can be done with Rebug Toolbox, or by enabling HEN. From there, navigate to Settings → Network Settings and hover over the Network Settings icon. Press and hold `L2 + L1 + R1 + R2 + L3 + DPAD-Down`. This will enable the Debug Settings section.

## **What is an Optical Drive Emulator \(ODE\)?**

An Optical Drive Emulator is a device that allows you to run game backups and homebrew on a PS3, without requiring a jailbroken console or Custom Firmware \(CFW\). Depending on the brand, it may support more models than CFW and may run on the latest OFW. See this page for more information.

## **Why are there multiple PS1/PS2 emulators?**

For PS1, a different emulator exists for discs and for PS1 Classic games from PSN.

| Emulator | Introduced In | Note |
| :--- | :--- | :--- |
| ps1\_emu | 1.00 OFW | Emulator for running PS1 discs. |
| ps1\_netemu | 1.70 OFW | Emulator for PS1 Classic games from PSN. |
| ps1\_newemu | 2.10 OFW | ??? |

For PS2, different iterations of hardware required different emulators and offsets. PS2 ISO launchers may have options to use a different emulator. In general, model-specific emulators have much better compatibility and performance, and the PS2 compatibility list is based on the ps2\_netemu.

| Emulator | Introduced In | Note |
| :--- | :--- | :--- |
| ps2\_emu | 1.00 OFW | For CECHA and CECHB, doesn't emulate Emotion Engine \(CPU\) or Graphics Synthesizer \(GPU\). |
| ps2\_gxemu | 1.50 OFW | For models CECHC and CECHE, doesn't emulate Graphics Synthesizer \(GPU\). |
| ps2\_softemu | 1.90 OFW | First iteration of full software emulator - deprecated in 4.01 OFW. |
| ps2\_netemu | 3.60^? | Emulator for PS2 Classics games from PSN. |

## **I'm interested in developing for the PS3. Where can I start?**

A. While this subreddit and Wiki is great for end-users, you are unlikely to find expert developer help here. You can see past and present research at the PS3 Devwiki, and get live help on the following IRC channels: \#psdevwiki, \#ps3dev, \#psl1ght. PSL1GHT is a community-made open source SDK used to develop homebrew.

