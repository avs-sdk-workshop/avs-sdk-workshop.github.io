---
title: 'Extra Credit'


layout: nil
---

### Go Headless

Now that you've got your AVS prototype running, you may want to get rid of the monitor, keyboard and mouse. You can do that by using SSH and VNC. Follow the instructions here to setup SSH and VNC.

**SSH** allows you to remotely access the command line of your Raspberry Pi from another computer (as long as they are both on the same network). This removes the requirement to have an external monitor connected to your Pi.

**VNC** is a graphical desktop sharing system that will allow you to remotely control the desktop interface of your Raspberry Pi from another computer. This will come in very handy as you get rid of the external monitor connected to your Pi.

---

#### SSH into the Raspberry Pi
**NOTE** SSH is **enabled by default** on Raspbian Jessie. If you run into problems getting SSH to work, make sure it’s enabled. This is done using the [raspi-config](https://www.raspberrypi.org/documentation/remote-access/ssh/README.md) utility.

So, let's SSH into your Raspberry Pi. To do that, you need to know the IP address of your Raspberry Pi.

Type this command into the terminal:

	hostname -I
	> 192.168.1.10 //this is an example Raspberry Pi’s IP - it would be different for you

If you’re on a Windows PC, follow the instructions here to [SSH Using windows](https://www.raspberrypi.org/documentation/remote-access/ssh/windows.md)

Now that you know the IP address of your Pi, you are ready to connect to it remotely using SSH. To do this, open the terminal utility on the computer you would like to connect from and type the following:

	ssh pi@<YOUR Raspberry Pi IP ADDRESS>

It will prompt you for your password. **NOTE**: the default password for the user pi is **raspberry**

Voila! You’re remotely connected to your Raspberry Pi. Now you can install all the utilities while connected remotely via SSH.

---

#### Install VNC Server

Open Terminal, and type:

	sudo apt-get install tightvncserver

**Start VNC Server**

To start VNC Server, type:

	tightvncserver

You'll be asked to set a password to access the Pi. You'll need this when you try to access the Pi from another computer, which we will be doing in a moment.

**Run VNCServer at Startup**

You want to make sure the VNC Server runs automatically after the Raspberry Pi reboots, so you don’t have to manually start it each time with the command *tightvncserver* through SSH. To do that, type the following in the terminal:

	cd /home/pi
	cd .config

Note the '.' at the start of the folder name. This makes it a hidden folder that will not show up when you type 'ls'.

	mkdir autostart
	cd autostart

Create a new configuration by typing the following command:

	nano tightvnc.desktop

Edit the contents of the file with the following text:

	[Desktop Entry]
	Type=Application
	Name=TightVNC
	Exec=vncserver :1
	StartupNotify=false

Type **ctrl-X** and then **Y**, and then press **Enter** to save the changes to the file.

That's it. The next time you **reboot**, the VNC server will restart automatically.

**Connecting to Raspberry Pi via VNC**

Please [download VNC viewer](https://www.realvnc.com/download/viewer) (available for Mac, Linux, Windows, and more), and follow the [instructions](https://www.raspberrypi.org/documentation/remote-access/vnc/) to connect to your Pi over VNC.

**You may now disconnect the Monitor, keyboard and mouse (if you like)**. Now with SSH (allows remote access to the terminal) and VNC (allows you to remote control the Raspberry Pi’s desktop interface) installed, the external monitor is optional. Feel free to disconnect it from the Raspberry Pi.
