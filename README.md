IVPORT Stereo Compute Module
---

Ivport Stereo CM is breakout board that you can plug a Raspberry Pi Compute Modules into. It comes with two Camera ports ant it enables you to use stereo recording and capturing modes simultaneously. It has also 10/100M Ethernet, dual USB 2.0 ports, Classic Raspberry Pi GPIO header, HDMI output, microSD slot and PoE (Power over Ethernet) support. It is also compatible with sorts of Raspberry Pi HATs.

![alt ivport stereo cm](https://raw.githubusercontent.com/ivmech/ivport-stereo-cm/master/images/ivport_scm_03.jpg)

### [Example Youtube Video](https://www.youtube.com/watch?v=e6cvI44fX18)

Raspberry Pi Compute Module, camera modules, camera ribbon cables, and power cable are needed.

### More information at [Wiki](https://github.com/ivmech/ivport-stereo-cm/wiki).


Getting Started
---

>On a Pi or Compute Module there are several files in the first FAT partition of the SD/eMMC that are binary 'Device Tree' files. These binary files (usually with extension .dtb) are compiled from human readable text descriptions (usually files with extension .dts) by the Device Tree compiler.

Copy precompiled **dt-blob.bin** binary file in first FAT partition of the microSD card.

>The Raspberry Pi uses a configuration file instead of the BIOS you would expect to find on a conventional PC. The system configuration parameters, which would traditionally be edited and stored using a BIOS, are stored instead in an optional text file named config.txt.

Add config values to the end of the **config.txt** file

```
start_x=1
gpu_mem=128
dtparam=i2c_vc=on
```
