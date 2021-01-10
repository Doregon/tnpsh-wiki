# TrueAncestor

[TrueAncestor](http://www.psx-place.com/ps3-news/3595/trueancestor-pkg-repacker-with-new-unpack-engine-version-220.html) is a multi-purpose program for extracting and repacking PKG files. You can also resign games to work on lower firmwares or [create debug (DEX) EBOOTs](https://www.reddit.com/r/ps3homebrew/wiki/eboots) (which requires [TrueAncestor 1.96](https://www.mediafire.com/?9xlivaj1dqap7ib) or lower) for real-time modding with a debugger such as [CCAPI](https://www.reddit.com/r/ps3homebrew/wiki/ccapi).

## Extracting a PKG


1. Place a PKG in the "pkg" folder inside the TrueAncestor directory

2. From the start screen in TrueAncestor; type 3 for "Unpack Pkg" and press enter

3. Type the number corresponding to your PKG from the list and press enter. The extracted package will be in the "game" folder inside the TrueAncestor directory


## Resigning and Repacking a PKG


1. Ensure you have your extracted PKG in the "game" folder inside the TrueAncestor directory

2. Under the Switch section,  check that Patch PARAM.SFO is set to [ON], if not, type in P and press enter

3. Under the Switch section,  check that Resign EBOOT.BIN is set to [ON], if not, type in R and press enter

4. Type 4 for "Repack Pkg" and press enter

5. Type the number corresponding to your game in the list and press enter. The newly built PKG will be in the "pkg" folder.