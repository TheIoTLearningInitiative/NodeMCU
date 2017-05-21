# Micro Python ESP8266

```sh
user@host:~$ make PORT=/dev/ttyUSB0 deploy
Use make V=1 or set BUILD_VERBOSE in your environment to increase build verbosity.
Writing build/firmware-combined.bin to the board
#@esptool.py --port /dev/ttyUSB0 write_flash 0 build/firmware-combined.bin
Connecting...
Erasing flash...
Took 0.87s to erase flash block
Wrote 51200 bytes at 0x00000000 in 4.9 seconds (82.9 kbit/s)...
Erasing flash...
Took 1.58s to erase flash block
Wrote 282624 bytes at 0x00010000 in 27.4 seconds (82.5 kbit/s)...
    
Leaving...
user@host:~$ su
password
root@host:~# minicom -D /dev/ttyUSB0
    
<reset>
```