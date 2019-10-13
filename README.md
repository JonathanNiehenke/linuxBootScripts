# custom init.d script

Scripts intended for debian boot

### Developed by:
Jonathan Niehenke

### Contained files:

- BT_Keyboard - init.d script for connecting a Bluetooth keyboard
- Readme.md - This file.

### Requires:
- root privilege of Linux system for installation

### How To:
1. First pair, connect and trust Bluetooth keyboard using bluetoothctl
2. Edit BT_Keyboard so the MAC variable matches the keyboards MAC address 
3. Move BT_Keyboard with root privilege to /etc/init.d
4.
    - For boot: With root privilege run `systemctl enable BT_Keyboard`
    - For service: With root privilege run `systemctl start BT_Keyboard`
