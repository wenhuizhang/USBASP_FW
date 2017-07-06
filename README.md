# USBASP_FW
firmware source code for usbasp atmega8/48/88


Firmware:
Flash "bin/firmware/usbasp.atmega88.xxxx-xx-xx.hex" or
"bin/firmware/usbasp.atmega8.xxxx-xx-xx.hex" to the used controller with a
working programmer (e.g. with avrdude, uisp, ...). Set jumper J2 to activate
USBasp firmware update function.
You have to change the fuse bits for external crystal (see "make fuses").
# TARGET=atmega8    HFUSE=0xc9  LFUSE=0xef
# TARGET=atmega48   HFUSE=0xdd  LFUSE=0xff
# TARGET=atmega88   HFUSE=0xdd  LFUSE=0xff
