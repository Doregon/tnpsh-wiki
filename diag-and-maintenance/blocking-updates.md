# Blocking Updates and PSN

## NP Environment

If you plan on playing offline exclusively, the easiest way to prevent your console and account from getting accidentally banned is to change the np-environment. The np-environment is an option that lets you choose which network your PS3 is connected to. By default it is set to PSN, while developers may use one of the 52 developer-only or Sony-internal networks if they are whitelisted. A full list of networks can be found [here](http://www.psdevwiki.com/ps3/Environments#Environments).

## Disabling or Re-Enabling PSN

Disabling PSN will mitigate any chance of getting banned by preventing your system from connecting to PSN. It will also prevent you from updating games via the XMB, but updating games through multiMAN will still work.

1. Enable the [QA flag](qa.md) on your console. If you are on Rebug, skip to step 4.
2. Navigate to the Settings column on the XMB and highlight "Network Settings".
3. Press and hold the following: DOWN \(D-Pad\)+ L1 + L2 + R1 + R2 + L3, this will enable Debug Settings.
4. Open Debug Settings and select "np-environment".
5. Type in "invalid" to disable PSN, or "np" to re-enable PSN, and then press Start.

