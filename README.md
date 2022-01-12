# AMD Ryzen Hackintosh

[![MacOS version](https://img.shields.io/badge/Catalina-10.15.7%2019H1323-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Bigsur-11.6.2%2020G313-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Monterey-12.2%20Beta2%2021D5039d-informational.svg)](https://www.apple.com/macos)\
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.7.7-informational.svg)](https://github.com/acidanthera/OpenCorePkg)\
[![GitHub](https://img.shields.io/github/license/sileshn/Ryzentosh?style=flat-square)](https://github.com/sileshn/Ryzentosh/blob/master/LICENSE)

## Important information
This EFI supports only MacOS versions catalina(10.15) and higher. Your system will not boot if you use this on Mojave and High Sierra.

<a href='https://postimg.cc/RJLKgSYB' target='_blank'><img src='https://i.postimg.cc/RJLKgSYB/Screenshot-2021-07-23-at-7-24-32-AM.png' border='0' alt='Screenshot-2021-07-23-at-7-24-32-AM'/></a> <a href='https://postimg.cc/Z9YZr0CC' target='_blank'><img src='https://i.postimg.cc/Z9YZr0CC/Screenshot-2021-12-08-at-12-33-41-PM.png' border='0' alt='Screenshot-2021-12-08-at-12-33-41-PM'/></a> <a href='http://postimg.cc/nMr8Nsjg' target='_blank'><img src='https://i.postimg.cc/nMr8Nsjg/Screen-Shot-2022-01-12-at-11.png' border='0' alt='Screen-Shot-2022-01-12-at-11'/></a>

## Disclaimer
Use at your own risk. I take no responsiblity if your rig explodes. Create unique SMBios values for your rig. Don't copy ones shown in the config.plist!!!

## Specification

| Component        | Model                                              |
| ---------------- | ---------------------------------------------------|
| CPU              | AMD Ryzen 7 2700                                   |
| MotherBoard      | Gigabyte B450 Aorus Elite                          |
| Wifi/Bluetooth   | Asus AX3000 Dual Band PCI-E WiFi 6 / Bluetooth 5.0 |
| OS Disk          | Gigabyte NVME GP-GSM2NE3256GNTD 256gb              |
| RAM              | 4x 8gb Corsair Vengeance Pro 32GB Ram              |
| GPU              | AMD Radeon RX570 4gb                               |
| Cooler    	   | Cooler master hyper 410r          		            |

## Working

* iCloud
* Bluetooth
* Ethernet
* Wifi
* iServices & drm
* Sleep

## Not Working ( only ones I have tried, there may be more )

* None apart from the known ones like sidecar afaik...

## Patches, Drivers & Kexts

* [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup)
* [AppleALC](https://github.com/acidanthera/AppleALC)
* [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)
* [Kernel Patches](https://github.com/AMD-OSX/AMD_Vanilla) ( Newer universal patches introduced in [this](https://github.com/sileshn/Ryzentosh/commit/adcb87fa003a0e77afaded014984a00ecb07b775) commit requires you to update the core count of your processor. For more information on this subject, click [here](https://github.com/AMD-OSX/AMD_Vanilla#read-me-first).)
* [Lilu](https://github.com/acidanthera/Lilu)
* [OpenCore](https://github.com/acidanthera/OpenCorePkg)
* [RadeonSensor](https://github.com/aluveitie/RadeonSensor)
* [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
* [RestrictEvents](https://github.com/acidanthera/RestrictEvents)
* [SMCAMDProcessor](https://github.com/trulyspinach/SMCAMDProcessor)
* [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen)

## Bootloader

I use OpenCore to multiboot Manjaro, Windows(10&11) and MacOS(Catalina, BigSur & Monterey)

[![10022018.png](https://i.postimg.cc/TwDYkvGy/10022018.png)](https://postimg.cc/cgdSHjvZ)

## Credits and links

* [OpenCore install guide](https://dortania.github.io/OpenCore-Install-Guide)
* [Hackintool](https://www.hackintosh-forum.de/forum/thread/38316-hackintool-ehemals-intel-fb-patcher)
* [OpenCore-Legacy-Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher)
* [OpenCore-Legacy-Patcher guide](https://dortania.github.io/OpenCore-Legacy-Patcher)
