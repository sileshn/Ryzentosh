# AMD Ryzen Hackintosh

[![MacOS version](https://img.shields.io/badge/Ventura-13.7.4-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Sonoma-14.7.8-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Sequoia-15.6.1-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Tahoe-26.0%20beta2-informational.svg)](https://www.apple.com/macos)\
[![OpenCore version](https://img.shields.io/badge/OpenCore-1.0.5-informational.svg)](https://github.com/acidanthera/OpenCorePkg)\
[![GitHub](https://img.shields.io/github/license/sileshn/Ryzentosh?style=flat-square)](https://github.com/sileshn/Ryzentosh/blob/master/LICENSE)

<a href="https://ibb.co/NnphwxbM"><img src="https://i.ibb.co/NnphwxbM/Screenshot-2025-02-23-at-4-33-40-PM.png" alt="Screenshot-2025-02-23-at-4-33-40-PM" border="0" /></a> <a href="https://ibb.co/PzCL5sbj"><img src="https://i.ibb.co/PzCL5sbj/Screenshot-2025-08-21-at-3-12-39-AM.png" alt="Screenshot-2025-08-21-at-3-12-39-AM" border="0"></a> <a href="https://ibb.co/Sw8VXCmK"><img src="https://i.ibb.co/Sw8VXCmK/Screenshot-2025-08-21-at-6-21-23-AM.png" alt="Screenshot-2025-08-21-at-6-21-23-AM" border="0"></a> <a href="https://ibb.co/XxCJNmjj"><img src="https://i.ibb.co/XxCJNmjj/Screenshot-2025-06-24-at-6-55-19-PM.png" alt="Screenshot-2025-06-24-at-6-55-19-PM" border="0"></a>
## Disclaimer
Use at your own risk. I take no responsiblity if your rig explodes. Create unique SMBios values for your rig. Don't copy ones shown in the config.plist!!!

## Important information
* This EFI supports only MacOS versions catalina(10.15) and higher. Your system will not boot if you use this on Mojave and High Sierra. As a result, there will be only 3 core count patches in this EFI instead of the usual 4.
* Incremental OTA updates starting from Ventura may fail and force you to download the full installer. This is probably due to BluetoolFixup kext. If you use BluetoolFixup in your setup like i do, you can overcome this issue by disabling the kext in your config.plist prior to running your updates and enable them back post updation.
* Universal patches introduced [here](https://github.com/sileshn/Ryzentosh/commit/adcb87fa003a0e77afaded014984a00ecb07b775) and updates for Ventura 13.3+ introduced [here](https://github.com/sileshn/Ryzentosh/commit/00aab441a0a8a0fbcc9532c7beb51bbec24d85cb) requires you to change the core count of your processor. More information can be found [here](https://github.com/AMD-OSX/AMD_Vanilla#read-me-first).
* Press spacebar to view additional options in the OC bootscreen.
* `Securebootmodel` should be set to `Disabled` for `Sonoma >= 14.4 & Sequoia` installs. You can change it back after the update.
* You will need to use [Helliport app](https://github.com/diepeterpan/HeliPort/releases/tag/v1.5.0) for wifi in Sequoia & Tahoe.
* AppleALC doesn't work on Tahoe.

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

* Audio doesn't work on Tahoe with AppleALC
* Sleep ( on Monterey )
* Sidecar
* Wifi ( itlwm works on Sequoia & Tahoe with Heliport app )

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

I use OpenCore to multiboot Solus, Windows 11 and MacOS(Monterey, Ventura, Sonoma, Sequoia) using the [BsxOc1](https://github.com/blackosx/BsxOc1) theme.

[![12024137.png](https://i.postimg.cc/63Tz2132/12024137.png)](https://postimg.cc/G8wv6Kvd)

## Credits and links

* [OpenCore install guide](https://dortania.github.io/OpenCore-Install-Guide)
* [Hackintool](https://www.hackintosh-forum.de/forum/thread/38316-hackintool-ehemals-intel-fb-patcher)
* [OpenCore-Legacy-Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher)
* [OpenCore-Legacy-Patcher guide](https://dortania.github.io/OpenCore-Legacy-Patcher)
