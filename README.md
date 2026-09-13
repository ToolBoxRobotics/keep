# keep


### Remove the sudo password prompt in the Ubuntu terminal
```bash
sudo visudo

ALL=(ALL:ALL) ALL     ->     %sudo ALL=(ALL:ALL) NOPASSWD:ALL
```

### Fix mouse lag on Ubuntu running on a Raspberry Pi
```bash
sudo nano /boot/firmware/cmdline.txt

usbhid.mousepoll=0 or 1

sudo apt update && sudo apt full-upgrade
sudo reboot
```

