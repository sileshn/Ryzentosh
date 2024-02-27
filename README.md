# AMD Ryzen Hackintosh

[![MacOS version](https://img.shields.io/badge/Bigsur-11.7.7-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Monterey-12.7.3-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Ventura-13.6.4-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Sonoma-14.4%20beta5-informational.svg)](https://www.apple.com/macos) \
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.9.8-informational.svg)](https://github.com/acidanthera/OpenCorePkg)\
[![GitHub](https://img.shields.io/github/license/sileshn/Ryzentosh?style=flat-square)](https://github.com/sileshn/Ryzentosh/blob/master/LICENSE)

<a href="https://postimg.cc/mcWSTcTC" target="_blank"><img src="https://i.postimg.cc/mcWSTcTC/Screenshot_2023-05-19_at_8.26.25_AM.png" alt="Screenshot_2023-05-19_at_8.26.25_AM"/></a> <a href="https://postimg.cc/VJPsThGw" target="_blank"><img src="https://i.postimg.cc/VJPsThGw/temp-Image26-C8-TR.jpg" alt="temp-Image26-C8-TR"/></a> <a href="https://postimg.cc/nMsHLxNZ" target="_blank"><img src="https://i.postimg.cc/nMsHLxNZ/temp-Image45-Yy-Gt.jpg" alt="temp-Image45-Yy-Gt"/></a> <a href="https://postimg.cc/yJ418v7F" target="_blank"><img src="https://i.postimg.cc/yJ418v7F/temp-Image3-V7bu-B.avif" alt="temp-Image3-V7bu-B"/></a>
## Disclaimer
Use at your own risk. I take no responsiblity if your rig explodes. Create unique SMBios values for your rig. Don't copy ones shown in the config.plist!!!

## Important information
* This EFI supports only MacOS versions catalina(10.15) and higher. Your system will not boot if you use this on Mojave and High Sierra. As a result, there will be only 3 core count patches in this EFI instead of the usual 4.
* Incremental OTA updates starting from Ventura may fail and force you to download the full installer. This is probably due to BluetoolFixup and IntelBluetoothFirmware kext's. If you use these kext's in your setup like i do, you can overcome this issue by disabling the kext's in your config.plist prior to running your updates and enable them back post updation.
* For Sonoma OTA updates to show up, you will need to add `revpatch=sbvmm` to your boot-args.
* Universal patches introduced [here](https://github.com/sileshn/Ryzentosh/commit/adcb87fa003a0e77afaded014984a00ecb07b775) and updates for Ventura 13.3+ introduced [here](https://github.com/sileshn/Ryzentosh/commit/00aab441a0a8a0fbcc9532c7beb51bbec24d85cb) requires you to change the core count of your processor. More information can be found [here](https://github.com/AMD-OSX/AMD_Vanilla#read-me-first).
* Wifi and bluetooth may or may not work on Sonoma depending on your hardware.
* Press spacebar to view additional options in the OC bootscreen.
* `IntelBTPatcher.kext`, `IntelBluetoothFirmware.kext` & `BlueToolFixup.kext` are disabled by default. Enable them if you want bluetooth support.
* `Securebootmodel` should be set to `Disabled` for Sonoma 14.4 beta installs.

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
* [Kernel Patches](https://github.com/AMD-OSX/AMD_Vanilla)
* [Lilu](https://github.com/acidanthera/Lilu)
* [OpenCore](https://github.com/acidanthera/OpenCorePkg)
* [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
* [OpenIntelWireless](https://github.com/OpenIntelWireless)
* [RestrictEvents](https://github.com/acidanthera/RestrictEvents)
* [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen)

## Bootloader

I use OpenCore to multiboot Manjaro, Windows(10&11) and MacOS(Catalina, BigSur, Monterey & Ventura)

[![04000725.png](https://i.postimg.cc/ZqdPpQj7/04000725.png)](https://postimg.cc/069JqcTD)

## Credits and links

* [OpenCore install guide](https://dortania.github.io/OpenCore-Install-Guide)
* [Hackintool](https://www.hackintosh-forum.de/forum/thread/38316-hackintool-ehemals-intel-fb-patcher)
* [OpenCore-Legacy-Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher)
* [OpenCore-Legacy-Patcher guide](https://dortania.github.io/OpenCore-Legacy-Patcher)
