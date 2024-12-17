# ffc2hdmi

**This is a WIP** ffc/csi to HDMI adapter base on the one found here : https://www.pcbway.com/project/shareproject/CSI_to_HDMI_Cable_Extension_Module.html  

You should be able to use this to connect a RPI camera module via a HDMI cable like so : RPI Csi camera connector > ffc2hdmi pcb > HDMI cable > ffc2hdmi pcb > Rpi camera CSI connector  

**This is a WIP and not guaranteed to work !**

## Changes 

Changes are as follows:

 * Replace part with wrong pitch (0.5mm vs 1mm) [Hirose FH12-15S-0.5SH](https://www.hirose.com/product/p/CL0586-0523-6-55?lang=en) with [Molex 522711579](https://www.molex.com/en-us/products/part-detail/522711579)
 * Use through hole parts
 * Change HDMI footprint to fit [Molex 2086581201](https://www.molex.com/en-us/products/part-detail/2086581003)

![PCB preview](ffc2hdmi.jpeg)


