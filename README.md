# RPi-Main
# Raspberry Pi project dumping ground and notes
# Headless SSH, by default RPi has SSH disabled *note* need to create ssh.txt file in root to enable ssh
# then create wpa_supplicant.conf with
country=US
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1

network={
scan_ssid=1
ssid="your_wifi_ssid"
psk="your_wifi_password"
}
Turn on RPi, connect via SSH clinet (Putty) with raspberrypi or raspberrypi.local depending on wireless or local CONX respectively
enter username pi and login
######
#Enable Desktop via VNC
sudo raspi-config for Win Bootup Setup like screen
Option 5 for interface options and P3 VNC to enable using arrow keys
Get VNC Viewer for PC you want to control RPi from
In VNC Viewer, use New Connection, enter either raspberrypi or raspberrypi.local (whichever was used to setup)
Double click on RPi setup in VNC Viewer and login
Profit?
*Note* Can update password via Putty by terminal command " passwd "
Once setup, only need RPi powered up and Putty or VNC depending on task
