## **BPI-M2S-bsp**
Banana Pi M2S/CM4 board bsp (u-boot 2015.1 & Kernel 4.9.241)

----------
**Prepare**

[Install Docker Engine](https://docs.docker.com/engine/install/) on your platform.

Get the docker image from [Sinovoip Docker Hub](https://hub.docker.com/r/sinovoip/bpi-build-linux-4.4/) , Build the source code with this docker environment.

Download source code

    $ git clone https://github.com/BPI-SINOVOIP/BPI-M2S-bsp
    $ git submodule update --init --recursive

 **Build**

Build all bsp packages, please run

    # ./build.sh bpi-m2s 1        //build m2s bsp
    # ./build.sh bpi-cm4 1        //build cm4 bsp

Target download packages in SD/bpi-m2s after build. Please check the build.sh and Makefile for detail

**Install**

Get the image from [bpi](http://wiki.banana-pi.org/Banana_Pi_BPI-M2S#Image_Release) and download it to the SD card. After finish, insert the SD card to PC

    # ./build.sh bpi-m2s 6        //install m2s bsp
    # ./build.sh bpi-cm4 6        //install cm4 bsp

Choose the type, enter the SD dev, and confirm yes, all the build packages will be installed to target SD card.
