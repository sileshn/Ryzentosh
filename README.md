# AMD Ryzen Hackintosh

[![MacOS version](https://img.shields.io/badge/Catalina-10.15.7%2019H1323-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Bigsur-11.6%2020G165-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Monterey-12.0%20Beta7%2021A5522h-informational.svg)](https://www.apple.com/macos)\
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.7.3-informational.svg)](https://github.com/acidanthera/OpenCorePkg)\
[![GitHub](https://img.shields.io/github/license/sileshn/Ryzentosh?style=flat-square)](https://github.com/sileshn/Ryzentosh/blob/master/LICENSE)

# Disclaimer
Use at your own risk. I take no responsiblity if your rig explodes. Create unique SMBios values for your rig. Don't copy ones shown in the config.plist!!!

[![Screenshot-2021-07-23-at-7-24-32-AM.png](https://i.postimg.cc/zv97X3SV/Screenshot-2021-07-23-at-7-24-32-AM.png)](https://postimg.cc/RJLKgSYB) [![Screenshot-2021-09-14-at-1-14-03-AM.png](https://i.postimg.cc/T3X6jd1N/Screenshot-2021-09-14-at-1-14-03-AM.png)](https://postimg.cc/4mwqsTzp) [![Screenshot-2021-09-22-at-7-09-40-AM.png](https://i.postimg.cc/6pJFXhLz/Screenshot-2021-09-22-at-7-09-40-AM.png)](https://postimg.cc/mtjm3CnF)

## Important information
This EFI supports only MacOS versions catalina(10.15) and higher. Your system will not boot if you use this on Mojave and High Sierra.

Monterey beta 6 software update may not show up if you have securebootmodel disabled in your config.plist. To get the update, change securebootmodel to the appropriate value based on your smbios ( [look here](https://dortania.github.io/OpenCore-Post-Install/universal/security/applesecureboot.html#securebootmodel) to find the values for your system ) and reboot. I had to choose j160 as my smbios is set to MacPro7,1. Make sure to change the securebootmodel back to disabled in the config.plist before the installer reboots the first time. DO NOT CHANGE THE SECURE BOOT VALUE IN BIOS.

To install Monterey Beta 7, you need to follow the steps below.

* Change securebootmodel to the appropriate value based on your smbios ( [look here](https://dortania.github.io/OpenCore-Post-Install/universal/security/applesecureboot.html#securebootmodel) ) and reboot for the update to show up.
* Install update after changing your smbios to iMac17,1 with securebootmodel set to disabled.( Booting from mackintosh HD )
* Change smbios to your original values and boot from your Monterey disk.

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

  Newer universal patches introduced in [this](https://github.com/sileshn/Ryzentosh/commit/adcb87fa003a0e77afaded014984a00ecb07b775) commit requires you to update the core count of your processor. For more information on this subject, click [here](https://github.com/AMD-OSX/AMD_Vanilla#read-me-first).
  
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
