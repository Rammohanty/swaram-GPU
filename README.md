# swaram-GPU
The GPU based implementation of the previous SWARAM architecture is detailed in this repository. This repository holds a few private repositories for the implementation of genome analysis using GPU based low powered embedded system. 
The configuration details for each node of the SWARAM-GPU architecture implementation are detailed in this section.
## Hardware Requirements
NVIDIA Jetson Nano - 8;
 eMMC 64GB (Minimum) -8;
 USB3.0 flash drive (128 GB) - 8;
 20 -port GB ethernet SWITCH -1;
Power Supply - 1;
 Network cable -16; and,
 An external hard drive for using as a storage for input reads.

## Single Node configuration
boot all Jetson Nano devices with LINUX OS;
 connect one flashdrive to each of the device;
 connect all NVIDIA Jetson Nano devices to the switch using the network cables;
and,
 configure the switch to establish a single ipaddress under which all the devices can
be grouped under.
The configuration needed to each of the NVIDIA Jetson Nano devices are:
 ensure DHCP automatic selection is selected;
 Enable SSH, genetrate ssh keys;
 copy the ssh keys to each and every devices to enable device to device easy communication;
 Mount swapfile, genomics folder, hard drive as storage and the flash drive as genstore on each of the device; and,
 copy the deduplication program to /genomics/sorting framework.
