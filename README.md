# AMD Ryzen Hackintosh

**MacOS version**: 11.0.1 beta  
**OpenCore version**: 0.6.3

[![Screenshot-2020-11-04-at-6-18-51-PM.png](https://i.postimg.cc/Cx12Z4Y7/Screenshot-2020-11-04-at-6-18-51-PM.png)](https://postimg.cc/JGfxvZsH)

## Specification

| Component        | Model                                  |
| ---------------- | -------------------------------------- |
| CPU              | AMD Ryzen 7 2700                       |
| MotherBoard      | MSI Pro VDH Max                        |
| OS Disk          | Kingston 240gb SSD                     |
| RAM              | 2x 8gb Corsair Vengeance Pro 16GB Ram  |
| GPU              | Nvidia Geforce GT710 2gb               |
| Cooler    	     | Stock AMD                              |

## Benchmarks

* [Cinebench](https://i.postimg.cc/c13FkMQ9/cinebench.png)
* [Geekbench](https://i.postimg.cc/YCdRLXH9/geekbench.png)

## Patches, Drivers & Kexts

* [Kernel Patches](https://github.com/AMD-OSX/AMD_Vanilla)
* [OpenRuntime](https://github.com/acidanthera/OpenCorePkg)
* [OpenCanopy](https://github.com/acidanthera/OpenCorePkg)
* [HfsPlusLegacy](https://github.com/acidanthera/OpenCorePkg) 
* [Lilu](https://github.com/acidanthera/Lilu)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
* [AppleALC](https://github.com/acidanthera/AppleALC)
* [AMDRyzenCPUPowerManagement](https://github.com/trulyspinach/SMCAMDProcessor)
* [AppleMCEReporterDisabler](https://github.com/acidanthera/OpenCorePkg)
* [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
* [AGPMInjector](https://github.com/Pavo-IM/AGPMInjector)
* [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
* [SMCAMDProcessor](https://github.com/trulyspinach/SMCAMDProcessor)


## Working

* Messaging
* iCloud
* Bluetooth
* Ethernet

## Bootloader

I use Manjaro's grub bootloader to triple boot Manjaro, Windows 10 and MacOSX.

[![Manjaro-grub.png](https://i.postimg.cc/HxGvhDMv/Manjaro-grub.png)](https://postimg.cc/t15zsc2F)

## Notes

Use at your own risk. I take no responsiblity if your rig explodes. SMBios values have not been updated in the config. You need to create them yourself.

Cedits and links:
* [OpenCore Desktop Guide](https://github.com/dortania/OpenCore-Desktop-Guide)
* [Hackintool](https://www.hackintosh-forum.de/forum/thread/38316-hackintool-ehemals-intel-fb-patcher/)
* [OC Builder](https://github.com/Pavo-IM/ocbuilder)
* [OC Configurator](https://mackie100projects.altervista.org/download-opencore-configurator/)
