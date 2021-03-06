# Monitoring

webMAN contains tools for system monitoring, which prove time and time again to be very helpful when you want to see what’s going on and whether or not you should take action immediately.

![](../../../../.gitbook/assets/wMAN-cpursx.png)

We'll divide this page into sections and explain each one. Keep in mind that this page updates every six seconds, rather than being updated every second.

The **red section** is where you'll find your system temperatures. Computer manufacturers commonly measure system temperatures in Celsius rather than Fahrenheit--although both are listed here. In this wiki and the subreddit, we use the Celsius measurement. Your console should see about 50-60 when the system is idle or 60-70 when it's in or has just come out of a game and in most cases, the RSX will be higher than the CPU.

* If you're sitting at higher-than-normal temperatures, you should consider following the steps described on the [Cooling Down](https://github.com/Doregon/tnpsh-wiki/tree/7a4cc24d492169a11c41d479a014c3d8ee706731/diag-and-maintenance/fix-cooling.md) page.
* For Phat users and 20xx owners: Even if you're sitting at the normal operating range, you should consider keeping your system a little cooler, maybe about 5 degrees. This can help prevent the Yellow Light of Death \(YLOD\) for _as long as possible_. I say as long due to the fact that cooling isn't the only factor that causes this issue--it's caused by any other major part of your system failing as well.
* The CPU can handle a maximum of 85 degrees. If you reach too high of a temperature, a notification saying "The system is too hot." will ask for you to shut down your console. webMAN tweaks this notification and says "MAXIMUM TEMPERATURE REACHED!" and promptly raises the fan speed to 100%.

The **blue section** monitors your storage and memory levels. PS3s come with 256MB of main memory and 256MB of graphics memory. The counter here only counts the main memory, which will be about 1-20MB free.

* \(Memory\) This is normal, and won't affect normal gameplay because of the graphics memory.
* \(Memory\)This can cause issues with webMAN's recording functionality if it's too low.
* \(Storage\) The system storage ticker is in MB rather than Gb, and it uses the binary counter rather than decimal. This can be a bit confusing if you use a Mac or another OS that thinks 1000MB = 1GB. In PS3 land, 1024MB = 1GB.
* \(System\) The ticker only shows the free storage space for the main drive, for external drives you can check them on the [Files](files.md) page.

The **green section** monitors your cooler speed. Pretty straightforward.

* The cooler speed is also shown as a hexadecimal.
* If the cooler controller is set to anything other than SYSCON,there will be a slider below the speed that you can drag to adjust. This will automatically change the controller to Manual, if it isn't already.
* The slider I mentioned above does not go under 20%. It shows a full 100%, but trying to drag it all the way to zero will set it at 20%.

The **blue section** shows power statistics and your console uptime.

* This data is gathered from the power supply unit--not the motherboard. If you replace your unit with a new one, all of these will reset.
* The clock icon is accompanied by the system's uptime, so how long it's been on. Note that uptime starts to count when the CPU is active--having your console in Standby doesn't add to the timer.
* The lightning option is accompanied by other power statistics, which are at this moment unknown.

And finally, the **yellow section** shows system software information.

* Your system's firmware version shows here, along with the exploit's name. PS3HEN users will see PS3HEN.
* Your system's PSID and IDPS also show here--hence why there's a dropdown rather than displaying them in full. Be careful if you're troubleshooting and need to send a screenshot to someone!
* webMAN's version and edition, i.e. webMAN MOD 1.47.29 \[Full\]. If you see \[Lite\] or nothing, we recommend running through the installation again.

