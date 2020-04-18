# install_aircrack
Script that installs Air Crack and the rtl8812au driver on a Raspberry Pi running Buster.

The script installs the required dependecies and then downloads the source code for Air Crack, compiles and installs it.

It then downloads, compiles and installs the driver for the rtl8812au.

Only tested on a Pi Zero W - YMMV

    chmod +x install_aircrack
    ./install_aircrack

# install_kismet
Script that installs Kismet

    chmod +x install_kismet
    ./install_kismet

# monitor_mode
On my Pi Zero W wlan0 is the built in wireless interface, the interface I put into monitor mode is wlan1. 

This script brings the interface `wlan1` down, pops it into monitor mode and then brings it back up - ready to be used by aircrack or kismet.

You will need to

    chmod +x monitor_mode

before you can run it.

	./monitor_mode

If your wireless interface is not called `wlan1` you will need to rename it in the script.
