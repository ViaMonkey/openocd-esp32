openocd-esp32
==============

* pre-built OpenOCD for windows from http://gnutoolchains.com/arm-eabi/openocd/
* Add in drivers zadig.exe and amontec driver for jtagkey2p. 
* use openocd-esp32.exe from terminal or add external tools in eclipse ide to debug esp target.

## Usage
In these examples the installation folder is on C:\openocd

usage jtag interface amontec jtagkey2p and board esp-wroom-32:

```
C:\openocd\bin\openocd-esp32.exe -s C:\openocd\share\openocd\scripts -f interface\ftdi\jtagkey2p.cfg -f board\esp-wroom-32.cfg
```

usage jtag devkit board esp32-wrover :

```
C:\openocd\bin\openocd-esp32.exe -s C:\openocd\share\openocd\scripts -f interface\ftdi\esp32_devkitj_v1.cfg -f board\esp32-wrover.cfg
```