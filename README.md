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
