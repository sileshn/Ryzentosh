# AMD Ryzen Hackintosh

[![MacOS version](https://img.shields.io/badge/macOS-10.15.7%2019H1321-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/macOS-11.5%20Beta%2020G5065a-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/macOS-12.0%20Beta%2021A5248p-informational.svg)](https://www.apple.com/macos)\
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.7.1-informational.svg)](https://github.com/acidanthera/OpenCorePkg)\
[![GitHub](https://img.shields.io/github/license/sileshn/Ryzentosh?style=flat-square)](https://github.com/sileshn/Ryzentosh/blob/master/LICENSE)

# Disclaimer
Use at your own risk. I take no responsiblity if your rig explodes. Create unique SMBios values for your rig. Don't copy ones shown in the config.plist!!!

[![Screenshot-2021-07-09-at-10-00-08-AM.png](https://i.postimg.cc/RVdkb4sP/Screenshot-2021-07-09-at-10-00-08-AM.png)](https://postimg.cc/3dyfk5Hp) [![Screenshot-2021-07-09-at-8-54-39-AM.png](https://i.postimg.cc/cJwT2c1s/Screenshot-2021-07-09-at-8-54-39-AM.png)](https://postimg.cc/5H9wFLFG) [![Screenshot-2021-06-30-at-7-16-10-AM.png](https://i.postimg.cc/c4kccDh7/Screenshot-2021-06-30-at-7-16-10-AM.png)](https://postimg.cc/JGJJr59t)

## Specification

| Component        | Model                                  |
| ---------------- | -------------------------------------- |
| CPU              | AMD Ryzen 7 2700                       |
| MotherBoard      | MSI Pro VDH Max                        |
| OS Disk          | Kingston 240gb SSD                     |
| RAM              | 2x 8gb Corsair Vengeance Pro 16GB Ram  |
| GPU              | Nvidia GT710 2gb                       |
| Cooler    	     | Cooler master hyper 410r               |

## Working

* iCloud
* Bluetooth
* Ethernet
* Wifi
* iServices

## Not Working ( only ones I have tried, there may be more )

* Drm related stuff ( Apple TV )
* Sleep

## Patches, Drivers & Kexts

* [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup)
* [AppleALC](https://github.com/acidanthera/AppleALC)
* [AppleMCEReporterDisabler](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip)
* [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)
* [Kernel Patches](https://github.com/AMD-OSX/AMD_Vanilla)
* [Lilu](https://github.com/acidanthera/Lilu)
* [OpenCore](https://github.com/acidanthera/OpenCorePkg)
* [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
* [RestrictEvents](https://github.com/acidanthera/RestrictEvents)
* [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen)

## Bootloader

I use OpenCore to multiboot Manjaro, Windows(10&11) and MacOS(Catalina, BigSur & Monterey)

[![30030721.png](https://i.postimg.cc/DwqcL1jn/30030721.png)](https://postimg.cc/75Z7yJrW)

## Credits and links

* [OpenCore Desktop Guide](https://github.com/dortania/OpenCore-Desktop-Guide)
* [Hackintool](https://www.hackintosh-forum.de/forum/thread/38316-hackintool-ehemals-intel-fb-patcher/)
* [OC Builder](https://github.com/Pavo-IM/ocbuilder)
* [OC Configurator](https://mackie100projects.altervista.org/download-opencore-configurator/)
