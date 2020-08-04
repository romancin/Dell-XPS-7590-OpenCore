# HP-ProDesk600-G5-mini-OpenCore
Repository to hold the files needed to install and run macOS on Dell XPS 7590

Change XX-MASKED-XX values in PlatformInfo section in config.plist file with your own values. Use [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS).

## Tested versions
OpenCore: 0.5.9

MacOS: macOS Catalina 10.15.6

## Configuration information
Key | Value
--- | ---
CPU | Intel Core i7 9750H
iGPU | Intel Graphics UHD 630
dGPU | Nvidia GeForce GTX 1650
Screen | Sharp 4K Display (non OLED)
RAM | Crucial DDR4 2666MHz 16GB *2
SSD | NVMe ADATA SX8200 Pro 1TB
Wireless | BCM94352Zz (DW1560)

##### Note before use
-**Please refer to this article first: [XPS 7590 1.6.0 UEFI: unlock undervolting and remove CFG lock](https://www.reddit.com/r/Dell/comments/fzv599/xps_7590_160_uefi_unlock_undervolting_and_remove/), for CFG Lock Unlock and undervolting capabilites! **

## Working
Internal Display with 4K sclaing options

Graphics Acceleration

Sound

All USB including USB-C port

Sleep

Bluetooth and WiFi (changing wireless card with DW1560)

Power Management with very good battery life (5-6 hours)

## Not Working
Bluetooth / WiFi  with stock killer card

Nvidia dGPU - No drivers are available, so it will probably never work. It is disabled by SSDT.

SD Card reader (no driver available)

## Log
-2020.8.4
  -First 100% working version

## Thanks
-Apple
-[@Acidanthera](https://github.com/acidanthera)
-[@gorquan](https://github.com/gorquan) This repo is based on your work, thank you very much :)
-[@tiger511](https://github.com/tiger511) For developing VoodooI2C fork for our laptop, awesome work, it works much better than current version by Acidanthera, thank you very much :)