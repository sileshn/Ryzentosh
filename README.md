# AMD Ryzen Hackintosh

[![MacOS version](https://img.shields.io/badge/Catalina-10.15.7-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Bigsur-11.7.2-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Monterey-12.6.3-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Ventura-13.3-informational.svg)](https://www.apple.com/macos) \
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.9.0-informational.svg)](https://github.com/acidanthera/OpenCorePkg)\
[![GitHub](https://img.shields.io/github/license/sileshn/Ryzentosh?style=flat-square)](https://github.com/sileshn/Ryzentosh/blob/master/LICENSE)

<a href="https://postimg.cc/WdzvYsny" target="_blank"><img src="https://i.postimg.cc/WdzvYsny/Screenshot-2022-07-13-at-11-29-46-AM.png" alt="Screenshot-2022-07-13-at-11-29-46-AM"/></a> <a href="https://postimg.cc/R643WRW2" target="_blank"><img src="https://i.postimg.cc/R643WRW2/Screenshot-2022-12-14-at-10-37-28-AM.png" alt="Screenshot-2022-12-14-at-10-37-28-AM"/></a> <a href='https://postimg.cc/dLNL9Yn3' target='_blank'><img src='https://i.postimg.cc/dLNL9Yn3/Screenshot-2023-02-17-at-4-53-10-AM.png' border='0' alt='Screenshot-2023-02-17-at-4-53-10-AM'/></a> <a href='https://postimg.cc/BjVShMt9' target='_blank'><img src='https://i.postimg.cc/BjVShMt9/Screenshot-2023-03-22-at-1-07-32-AM.png' border='0' alt='Screenshot-2023-03-22-at-1-07-32-AM'/></a>

## Disclaimer
Use at your own risk. I take no responsiblity if your rig explodes. Create unique SMBios values for your rig. Don't copy ones shown in the config.plist!!!

## Important information
* This EFI supports only MacOS versions catalina(10.15) and higher. Your system will not boot if you use this on Mojave and High Sierra. As a result, there will be only 3 core count patches in this EFI instead of the usual 4.
* Universal patches introduced [here](https://github.com/sileshn/Ryzentosh/commit/adcb87fa003a0e77afaded014984a00ecb07b775) and updates for Ventura 13.3+ introduced [here](https://github.com/sileshn/Ryzentosh/commit/00aab441a0a8a0fbcc9532c7beb51bbec24d85cb) requires you to change the core count of your processor. More information can be found [here](https://github.com/AMD-OSX/AMD_Vanilla#read-me-first).
* Press spacebar to view additional options in the OC bootscreen.

## Specification

| Component        | Model                                              |
| ---------------- | ---------------------------------------------------|
| CPU              | AMD Ryzen 5 3600                                   |
| MotherBoard      | Gigabyte B450 Aorus Elite                          |
| Wifi/Bluetooth   | Fenvi T919                                         |
| OS Disk          | Gigabyte NVME GP-GSM2NE3256GNTD 256gb              |
| RAM              | 4x 8gb Corsair Vengeance Pro 32GB Ram              |
| GPU              | AMD Radeon RX570 4gb                               |
| Cooler    	   | Arctic Freezer A35 A-RGB          		            |

## Working

* iCloud
* Bluetooth
* Ethernet
* Wifi
* iServices & drm

## Not Working ( only ones I have tried, there may be more )

* Sleep ( on Monterey )
* Sidecar

## Patches, Drivers & Kexts

* [AppleALC](https://github.com/acidanthera/AppleALC)
* [AppleMCEReporterDisabler](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip)
* [Kernel Patches](https://github.com/AMD-OSX/AMD_Vanilla)
* [Lilu](https://github.com/acidanthera/Lilu)
* [OpenCore](https://github.com/acidanthera/OpenCorePkg)
* [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
* [RestrictEvents](https://github.com/acidanthera/RestrictEvents)
* [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen)

## Bootloader

I use OpenCore to multiboot Manjaro, Windows(10&11) and MacOS(Catalina, BigSur, Monterey & Ventura)

[![13060127.png](https://i.postimg.cc/nLFcQJvB/13060127.png)](https://postimg.cc/CR2VW9rx)

## Credits and links

* [OpenCore install guide](https://dortania.github.io/OpenCore-Install-Guide)
* [Hackintool](https://www.hackintosh-forum.de/forum/thread/38316-hackintool-ehemals-intel-fb-patcher)
* [OpenCore-Legacy-Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher)
* [OpenCore-Legacy-Patcher guide](https://dortania.github.io/OpenCore-Legacy-Patcher)
