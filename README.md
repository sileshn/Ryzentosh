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
| Cooler    	   | Stock AMD                              |


## Patches, Drivers & Kexts

- [Patchs] AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
- [Driver] OpenRuntime
- [Driver] OpenCanopy
- [Driver] HfsPlusLegacy
- [Kext] Lilu
- [Kext] WhateverGreen
- [Kext] AppleALC
- [Kext] AMDRyzenCPUPowerManagement
- [Kext] AppleMCEReporterDisabler
- [Kext] AGPMInjector
- [Kext] RealtekRTL8111
- [Kext] SMCAMDProcessor


## Working

- [x] Messaging
- [x] iCloud
- [x] Bluetooth
- [x] Ethernet

## Bootloader

I use Manjaro's grub bootloader to triple boot Manjaro, Windows 10 and MacOSX.

[![Manjaro-grub.png](https://i.postimg.cc/HxGvhDMv/Manjaro-grub.png)](https://postimg.cc/t15zsc2F)