# Real-Time Mods

Game modding boils down to being able to load cheats and change variables within a game at your will. There are various options for modding PS3 games. If you are just looking to use simple cheats for an offline game, it may be easier to use [Artemis](../game-mods-cheats/artemis/README.md). Note that modding online games will put you at a higher risk of a ban.

One modding option is to use a debugger framework such as [CCAPI](ccapi/README.md), [TMAPI](tmapi/README.md) or [PS3MAPI](ps3mapi/README.md) which will allow you to use a debugger on your PC to real-time edit values of a game similar to CheatEngine (or use a tool that does so).

A second option is to use a pre-built set of mods, often packaged as a "mod menu", which comes as an EBOOT, SPRX, and/or a RPF.

EBOOT/SPRX/RPF Mods

Check to make sure that your desired mod is compatible with your firmware type (CEX or DEX). It is recommended to add ".bak" to the end of your original file names in case you need to revert back. The process for each mod is as follows:

* EBOOTs: Transfer your modded EBOOT via [FTP](../pc-tools/ftp-client.md) to: /dev_hdd0/game/<TitleID>/USRDIR/.

* SPRX: Transfer your SPRX via [FTP](../pc-tools/ftp-client.md) to: /dev_hdd0/tmp/

* RPF: Transfer your modded RPF via [FTP](../pc-tools/ftp-client.md) to: /dev_hdd0/game/<TitleID>/USRDIR/.