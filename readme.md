<p align="center"><img src="doc/img/realsense.png" width="80%" /><br><br></p>

-----------------

Linux | Windows |
-------- | ------------ |
[![Build Status](https://travis-ci.org/IntelRealSense/librealsense.svg?branch=master)](https://travis-ci.org/IntelRealSense/librealsense) | [![Build status](https://ci.appveyor.com/api/projects/status/y9f8qcebnb9v41y4?svg=true)](https://ci.appveyor.com/project/ddiakopoulos/librealsense) |

**Intel® RealSense™ Cross Platform SDK** is a cross-platform library (Linux, Windows, Mac) for working with Intel® RealSense™ depth cameras.
Developer kits containing the necessary hardware to use this library are available for purchase at [this link](http://click.intel.com/realsense.html). 

[Whats new?](./doc/rs400_support.md) - Summary of changes in librealsense2, including RS400 support, API changes and new functionality.

## Table of Contents
* Installation Guides:
  * [Linux](./doc/installation.md)
  * [Windows](./doc/installation_windows.md)
  * [Mac OS X](./doc/installation_osx.md)
* [Useful Links](#useful-links)
* [Documentation](#documentation)
* [Functionality](#functionality)
* [Compatible Devices](#compatible-devices)
* [Compatible Platforms](#compatible-platforms)
* [Integrations](#integrations)
* [License](#license)


## Functionality

1. Native streams: depth, color, infrared, fisheye, motion-tracking.
2. Synthetic streams: depth aligned to color and vice versa, pointcloud.
3. Intrinsic/extrinsic calibration information.
4. Majority of hardware-specific functionality for individual camera generations (UVC XU controls).
5. Multi-camera capture across heterogeneous camera architectures

## Compatible Devices

1. RealSense SR300
2. RealSense RS400 series

## Compatible Platforms

The library is written in standards-conforming C++11 and relies only on the C89 ABI for its public interface. It is developed and tested on the following platforms:

1. Ubuntu 14/16 LTS (GCC 4.9 toolchain)
2. Windows 10 (Visual Studio 2015 Update 3)
3. Mac OS X 10.7+ (Clang toolchain) **Temporarily unavailable**

## Hardware Requirements
Developer kits containing the necessary hardware to use this library are available for purchase at [this link](http://click.intel.com/realsense.html). In addition, several consumer tablets and laptops with integrated cameras may also function, such as the [HP Spectre x2 with R200](http://store.hp.com/us/en/ContentView?storeId=10151&langId=-1&catalogId=10051&eSpotName=new-detachable).

Developer kits **require** USB 3.0. RealSense™ cameras do not provide backwards compatibility with USB 2.0. Not all USB host chipsets are compatible with this library, although it has been validated with recent generations of the Intel Host Controller chipset. An exhaustive list of incompatible hardware is not presently provided. On x86, a Haswell or newer architecture is recommended.

For small-form factor usages, this library has been demonstrated to work on the following boards:
  * [UP Board](http://www.up-board.org/kickstarter/up-intel-realsense-technology/)
  * [Intel Joule](https://newsroom.intel.com/chip-shots/make-amazing-things-happen-iot-entrepreneurship-intel-joule/)

## Integrations

The library has been integrated with a number of third-party components and operating systems. While most of these projects are not directly supported by the team, they are useful resources for users of this library.

  * [Robotic Operating System](https://github.com/intel-ros/realsense) (Intel Supported; R200, F200, SR300 all supported)
  * [Yocto / WindRiver Linux](https://github.com/IntelRealSense/meta-intel-librealsense)
  * [Arch Linux](https://aur.archlinux.org/packages/librealsense/)

Additional language bindings (experimental, community maintained):
  * [Java (generated by JavaCPP)](https://github.com/poqudrof/javacpp-presets/tree/realsense-pull)

## License

This project is licensed under the Apache License, Version 2.0 - see the [LICENSE](LICENSE) file for details