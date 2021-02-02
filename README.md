[![OpenCore](https://img.shields.io/badge/OpenCore-v0.6.5-blue.svg)](https://github.com/acidanthera/OpenCorePkg)
[![MacOS-Stable](https://img.shields.io/badge/MacOS-10.15.7-brightgreen.svg)](https://www.apple.com/macos/catalina/)
![STATUS](https://img.shields.io/badge/STATUS-stable-green.svg)

# Introduction
This is my first hackintosh project. This hackintosh configuration is built for ASRock X370M-HDV motherboard. This repository is intended for educational purpose. Personally, I don't have much money for buying mac device, so... this is my approach.

# Disclaimer
Please read entire guide from Dortania OpenCore Guides and this ReadMe before you using this config. I am not responsible for any damage. If you want to improve this repo, please make issue or pull request. Any help would be greatly appreciated.

# Configuration
#### SMBIOS: iMacPro1,1
 ### Hardware
| Category      | Component        |
|---------------|------------------|
| CPU           | AMD Ryzen 1600   |
| Motherboard   | ASRock X370M-HDV |
| GPU           | AMD Radeon RX560 |
| SSD           | ADATA SX8200PNP  |
| Wireless Card | BCM93450ZAE      |
*note : Bluetooth cable not plugged in
 
 ### BIOS Configuration
| Settings          | Value     |
|-------------------|-----------|
| fastboot          | disabled  |
| Secure Boot       | disabled  |
| CSM               | disabled  |
| SATA Mode         | AHCI      |
| Above 4G decoding | disabled  |
*note : Above 4G decoding makes windows unstable

 ### Kext
| Name          | Version    |
|-------------------|-----------|
| [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup)          | 2.1.2  |
| [AppleALC](https://github.com/acidanthera/AppleALC)       | 1.5.6  |
| [Lilu](https://github.com/acidanthera/Lilu)               | 1.5.0  |
| [RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)         | 2.3      |
| [VirtualSMC](https://github.com/acidanthera/VirtualSMC)| 1.1.9 |
| [WhateverGreen](https://github.com/acidanthera/WhateverGreen) | 1.4.6 |


# Working & Not-Working
### Working
- Wi-Fi
- GPU Acceleration
- Sleep/Wake
- Shutdown - Restart
- USB Port
- Sound Output
- etc.
 
### Not-Working
- Apple Native Virtualization `use virtualbox instead`
- Sound Input `use usb DAC instead`
# Credits
This build wouldn't happen without these people: 
- [Dortania](https://github.com/dortania) for OpenCore Guide
- [headkaze](https://github.com/headkaze) for Hackintool 
- [Acidanthera](https://github.com/acidanthera) for too many things
- [OpenCore project](https://github.com/OpenCorePkg) for the bootloader
- [Mieze](https://github.com/Mieze) for the RTL8111 driver

