UbuntuOnAndroid
===============

A mostly harmless, experimental full-sized ARM-compiled version of Ubuntu, running on Android in the background (you can use your phone, while it's running). It
automatically starts its own VNC server, so you can access the GUI from anywhere. You need a rooted and perhaps, a S-OFFed device for this.

1. Put both of the bootubuntu and exitu scripts in the /system/bin/ folder of your device and chmod +x them.
2. Put the ubuntu.img (I'll upload this later) file in a /sdcard/Ubuntu/ folder (you may change the folder, using the $uloc variables in both scripts).
3. Run bootubuntu (it will chroot in Ubuntu and if all is well, automatically start the VNC server).
	* DON'T exit the terminal, because as of yet, I haven't found a way to get back in it.
4. When you're done with Ubuntu, kill the VNC server from within Ubuntu (either through the VNC viewer, or the terminal) and run the exitu command on the Android 
terminal.
	* If you don't kill the VNC server, you probably won't be able to umount and kill Ubuntu. If this happens, just restart your device.
	* The Ubuntu uses the loop99 process. You can see if it's running, by using the `ps` command on your Aandroid terminal.


Tested on HTC Desire and Nexus One.

I take no responsibility for bricked devices, thermonuclear war, or you getting fired, because your alarm app failed. Use these scripts at your own discretion.
