# ffc2hdmi

**This is a WIP** ffc/csi to HDMI adapter base on the one found here : https://www.pcbway.com/project/shareproject/CSI_to_HDMI_Cable_Extension_Module.html  

You should be able to use this to connect a RPI camera module via a HDMI cable like so : RPI Csi camera connector > ffc2hdmi pcb > HDMI cable > ffc2hdmi pcb > Rpi camera CSI connector  

![PCB](https://raw.githubusercontent.com/ABelliqueux/ffc2hdmi/refs/heads/main/ffc2hdmi-pcb.jpg)  

## Limitations

I have tested this PCB successfully with a RPI 4B+ and a raspicam V3.  
Currently, the **maximum length of the HDMI cable is 1.8M**. I tested with 3M and 10M cables and got timing error messages from libcamera.  
If you can test with other hardware and find that it works, please submit an issue stating your HW (rpi model, cam model and HDMI cable length.)  

The current length is enough for my usecase, but if you find a way to user longer cables, please open an issue stating your solution. I have spare PCBs and can do some tests (changing resistors/capacitors value ?).

## Parts needed 

 * This PCB x 2
 * 1.6Kohm resistor x 4
 * 100nf (0.1uf) ceramic capacitor x 2
 * FFC ([Molex 522711579](https://www.molex.com/en-us/products/part-detail/522711579)) connector x 2
 * HDMI [Molex 2086581201](https://www.molex.com/en-us/products/part-detail/2086581003) connector x 2
 * A HDMI cable (1.8M max)

## How do I get the PCB ?

You should be able to [grab the gerber files in this repo](https://github.com/ABelliqueux/ffc2hdmi/raw/refs/heads/main/ffc2hdmi_fab.zip) and use your favorite PCB maker like Jlcpcb or pcbway.

## Changelog

Changes are as follows:

 * Replace part with wrong pitch (0.5mm vs 1mm) [Hirose FH12-15S-0.5SH](https://www.hirose.com/product/p/CL0586-0523-6-55?lang=en) with [Molex 522711579](https://www.molex.com/en-us/products/part-detail/522711579)
 * Use through hole parts
 * Change HDMI footprint to fit [Molex 2086581201](https://www.molex.com/en-us/products/part-detail/2086581003)
 * Mounting holes are now 2.5mm instead of 2mm.

![PCB preview](https://raw.githubusercontent.com/ABelliqueux/ffc2hdmi/refs/heads/main/ffc2hdmi.jpg)  
![PCB preview](https://raw.githubusercontent.com/ABelliqueux/ffc2hdmi/refs/heads/main/ffc2hdmi_sch.png)

