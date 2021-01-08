#PS3MAPI
___

PS3 Manager API is a framework similar to TMAPI or CCAPI that is included in the [Cobra](https://www.reddit.com/r/ps3homebrew/wiki/mamba) and [MAMBA](https://www.reddit.com/r/ps3homebrew/wiki/mamba) payloads. It allows you to read and write values and addresses in RAM in real-time using a supported device over the local network. It's typically used for debugging and real time game modding. Note that in order to modify games, you must first convert their EBOOT to a [debug EBOOT](https://www.reddit.com/r/ps3homebrew/wiki/eboots). MAPI is supported on both CEX and DEX firmwares.

It's features include:

- Getting process and process name by PID
- Make all memory writable for any process
- Getting process module and module name by prxid
- Load and unload a process module
- Get and Unload VSH plugins by name
- Disable and check any syscall 
- Remove cobra/mamba hook
- Get and set IDPS/PSID at any time

___


Forcing Tools to Use MAPI
---
Often times, PC tools are built solely for CCAPI. You can force them to use MAPI by extracting the PS3Lib.dll into the tool's folder from [Fake CCAPI](http://www.mediafire.com/download/znig9z0dsbg6x7k/Fake_CCAPI.rar).


A set of demo tools built specifically for MAPI can be found [here](http://www.mediafire.com/download/la132l9vfpb1fba/PS3M_API_Demo_Tools.rar).

Using MAPI via Browser
---

If you have Rebug firmware or WebMAN-MOD installed, you can use MAPI with any device on your network by browsing to: [your.ps3s.ip.here/home.ps3mapi](https://www.reddit.com/r/ps3homebrew/wiki/mapi)


CID Stealer Protection
---

If you are planning on using a mod tool on your PC in conjunction with MAPI, it's a good idea to block the program's Internet access so it can't steal your ConsoleID (CID) and upload it to someone else if it is malicious. You can do this with the following process on Windows:

1. Click on your Start Menu and type "Windows Firewall" and select the option that pops up.

2. Select Advanced Settings → Outbound Rules (left side) → New Rule (right side).

3. Follow the wizard and select the .exe file of your mod tool and block it from Domain, Public, and Private networks.