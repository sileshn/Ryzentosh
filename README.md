# AMD Ryzen Hackintosh

**MacOS version**: 11.1 beta2  
**OpenCore version**: 0.6.4

# Disclaimer
Use at your own risk. I take no responsiblity if your rig explodes. Create unique SMBios values for your rig. Don't copy ones shown in the config.plist!!!

[![bigsur.png](https://i.postimg.cc/C1rTHPNV/bigsur.png)](https://postimg.cc/N9XzQxSN)

## Specification

| Component        | Model                                  |
| ---------------- | -------------------------------------- |
| CPU              | AMD Ryzen 7 2700                       |
| MotherBoard      | MSI Pro VDH Max                        |
| OS Disk          | Kingston 240gb SSD                     |
| RAM              | 2x 8gb Corsair Vengeance Pro 16GB Ram  |
| GPU              | Radeon RX570 4gb | Nvidia GT710 2gb    |
| Cooler    	   | Cooler master hyper 410r               |

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
* [AirportBrcmFixup](https://github.com/acidanthera/airportbrcmfixup/releases)
* [BrcmFirmwareData](https://github.com/acidanthera/BrcmPatchRAM)
* [BrcmPatchRAM3](https://github.com/acidanthera/BrcmPatchRAM)
* [BrcmBluetoothInjector](https://github.com/acidanthera/BrcmPatchRAM)
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

## Cedits and links

* [OpenCore Desktop Guide](https://github.com/dortania/OpenCore-Desktop-Guide)
* [Hackintool](https://www.hackintosh-forum.de/forum/thread/38316-hackintool-ehemals-intel-fb-patcher/)
* [OC Builder](https://github.com/Pavo-IM/ocbuilder)
* [OC Configurator](https://mackie100projects.altervista.org/download-opencore-configurator/)
