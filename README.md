# AMD Ryzen Hackintosh

[![MacOS version](https://img.shields.io/badge/Catalina-10.15.7-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Bigsur-11.7.1-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Monterey-12.6.1-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Ventura-13.1%20Beta4-informational.svg)](https://www.apple.com/macos) \
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.8.7-informational.svg)](https://github.com/acidanthera/OpenCorePkg)\
[![GitHub](https://img.shields.io/github/license/sileshn/Ryzentosh?style=flat-square)](https://github.com/sileshn/Ryzentosh/blob/master/LICENSE)

<a href="https://postimg.cc/WdzvYsny" target="_blank"><img src="https://i.postimg.cc/WdzvYsny/Screenshot-2022-07-13-at-11-29-46-AM.png" alt="Screenshot-2022-07-13-at-11-29-46-AM"/></a> <a href="https://postimg.cc/18gWcJWG" target="_blank"><img src="https://i.postimg.cc/18gWcJWG/Screenshot-2022-10-26-at-8-48-36-AM.png" alt="Screenshot-2022-10-26-at-8-48-36-AM"/></a> <a href='https://postimg.cc/p9g0yzR2' target='_blank'><img src='https://i.postimg.cc/p9g0yzR2/Screenshot-2022-10-26-at-7-16-44-AM.png' border='0' alt='Screenshot-2022-10-26-at-7-16-44-AM'/></a> <a href='https://postimg.cc/5jM6D4ms' target='_blank'><img src='https://i.postimg.cc/5jM6D4ms/Screenshot-2022-12-02-at-4-19-11-PM.png' border='0' alt='Screenshot-2022-12-02-at-4-19-11-PM'/></a>

## Disclaimer
Use at your own risk. I take no responsiblity if your rig explodes. Create unique SMBios values for your rig. Don't copy ones shown in the config.plist!!!

## Important information
* This EFI supports only MacOS versions catalina(10.15) and higher. Your system will not boot if you use this on Mojave and High Sierra.
* Ventura incremental OTA updates may fail post beta1 and force you to download the full installer. This is probably due to BluetoolFixup and IntelBluetoothFirmware kext's. If you use these kext's in your setup like i do, you can overcome this issue by disabling the kext's in your config.plist prior to running your updates and enable them back post updation.

## Specification

| Component        | Model                                              |
| ---------------- | ---------------------------------------------------|
| CPU              | AMD Ryzen 5 3600                                   |
| MotherBoard      | Gigabyte B450 Aorus Elite                          |
| Wifi/Bluetooth   | Asus AX3000 Dual Band PCI-E WiFi 6 / Bluetooth 5.0 |
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
* [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)
* [Kernel Patches](https://github.com/AMD-OSX/AMD_Vanilla) ( Newer universal patches introduced in [this](https://github.com/sileshn/Ryzentosh/commit/adcb87fa003a0e77afaded014984a00ecb07b775) commit requires you to update the core count of your processor. For more information on this subject, click [here](https://github.com/AMD-OSX/AMD_Vanilla#read-me-first).)
* [Lilu](https://github.com/acidanthera/Lilu)
* [OpenCore](https://github.com/acidanthera/OpenCorePkg)
* [OpenIntelWireless](https://github.com/OpenIntelWireless)
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
