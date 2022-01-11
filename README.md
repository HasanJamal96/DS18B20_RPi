	Sensor	        RPi

	Red Wire        5v
	Black Wire	GND
	Yellow Wire    GPIO 4

Enable ONE-WIRE Interface:
Open terminal and run the following commands.
	
	# sudo nano /boot/config.txt

New window will appear add this line at the end of the file then press ctrl+x then press y then enter to save.

	dtoverlay=w1-gpio

Now reboot RPi.
After reboot, open terminal and run the following commands.
	
	$ sudo modprobe w1-gpio
	$ sudo modprobe w1-therm
