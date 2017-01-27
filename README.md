# hp50codes

This is a personal repository for some small programs for my HP50g. In loving memory of those from my college years I lost on an old SD card.

The programs are written in UserRPL. Because RPN rocks.
# List
## nuclear
Includes some variations of the semi-empirical mass formula, some constants and related stuff.

## astcoor
Includes some formulae for astronomical coordinate conversion. Angles are (supposed to be) picked from the correspoding quadrant.
Calculator must be set in degrees for some of them to work.
Order convention is the same as in the textbook I used.

# Notes on connectivity
Install ckermit
```
sudo pacman -S ckermit
```
Physically connect with usb cable and check with `dmesg | tail`.
Now `sudo ckermit -l /dev/ttyUSB0` or something similar.
In kermit you should first
```
set carrier-watch off
robust
```
This can also be set in a .kermrc file.

- To send a file to the calculator LSHIFT+LEFT PAD to put it in server mode and then `send foo`.
- To recieve from the calculator set the computer in server mode by running `server` and then send the file with the SEND command or from the APPS menu.
