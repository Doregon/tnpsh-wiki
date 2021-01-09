# ProDG TMAPI

PS3 Manager API is a framework similar to TMAPI or CCAPI that is included in the [Cobra](https://www.reddit.com/r/ps3homebrew/wiki/mamba) and [MAMBA](https://www.reddit.com/r/ps3homebrew/wiki/mamba) payloads. It allows you to read and write values and addresses in RAM in real-time using a supported device over the local network. It's typically used for debugging and real time game modding. Note that in order to modify games, you must first convert their EBOOT to a [debug EBOOT](https://www.reddit.com/r/ps3homebrew/wiki/eboots). MAPI is supported on both CEX and DEX firmwares.

Its features include:

* Getting process and process name by PID
* Make all memory writable for any process
* Getting process module and module name by prxid
* Load and unload a process module
* Get and Unload VSH plugins by name
* Disable and check any syscall 
* Remove cobra/mamba hook
* Get and set IDPS/PSID at any time

