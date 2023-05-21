# OpenCore 0.9.2 for Ryzentosh

**OpenCore : 0.9.2**

**macOS ：Ventura 13.4**

**SMBIOS : MacPro7,1**

### Specification

| **Component**    | **Model**                  |
| ---------------- | -------------------------- |
| CPU              | AMD Ryzen 5 3500X @ 4.2Ghz |
| Motherboard      | MSI B550M PRO-VDH WIFI     |
| RAM              | HyperX 2x8GB DDR4 @ 2933MHz|
| Audio Chipset    | Realtek ALC897 (layout-id=11)|
| GPU              | GIGABYTE RX 5500XT 4GB     |
| Ethernet         | Realtek RTL8168            |
| WiFi & Bluetooth | Intel Dual-Band Wireless-AC 3168|
| OS Disk(NMVe)    | Kingspec NE-1TB            |

## Compatability macOS versions
 - Catalina (10.15.2-10.15.7)
 - Big Sur (11.x)
 - Monterey (12.x)
 - Ventura (13.x)

## Instructions
  1. Make your USB installer with [**this guide**](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)
  2. Clone the repository and paste "BOOT" and "OC" directories into your's pendrive "EFI" folder
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as the model select **MacPro7,1**. 

**DON'T USE SMBIOS FROM THIS CONFIG, IT NEEDS TO BE UNIQUE FOR EACH INSTALLATION**
  4. Boot it

## :white_check_mark: Working:
- [x] CPU power management.
- [x] Graphics acceleration.
- [x] Keyboard & Mouse
- [x] USB ports.
- [x] HDMI video & audio output.
- [x] Ethernet.
- [x] Audio (Internal speakers, 3.5mm headphone jack).
- [x] Internal microphone.
- [x] iCloud & App Store.
- [x] iMessage & FaceTime.

## :x: Not working

- Hypervisor.framework (VirtualBox and XCode iOS emulator works)
- Microphone (If you are use USB microphone or audio card it's probably solve this issue)
- WiFi (In my case)

## Kexts

- [[Kext] Lilu](https://github.com/acidanthera/Lilu)
- [[Kext] VirtualSMC](https://github.com/acidanthera/VirtualSMC)
- [[Kext] WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- [[Kext] AppleALC](https://github.com/acidanthera/AppleALC)
- [[Kext] RealtekRTL8111](https://bitbucket.org/RehabMan/os-x-realtek-network/downloads/)
- [[Kext] AGPMInjector](https://github.com/Pavo-IM/AGPMInjector)
- [[Kext] AirportItlwm](https://github.com/OpenIntelWireless/itlwm)
- [[Kext] AMDRyzenCPUPowerManagement](https://github.com/trulyspinach/SMCAMDProcessor)
- [[Kext] AppleMCEReporterDisabler](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip)
- [[Kext] BlueToolFixup](https://github.com/acidanthera/BrcmPatchRAM)
- [[Kext] Innie](https://github.com/cdf/Innie)
- [[Kext] IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)
- [[Kext] RadeonSensor](https://github.com/aluveitie/RadeonSensor)
- [[Kext] RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
- [[Kext] RestrictEvents](https://github.com/acidanthera/RestrictEvents)
- [[Kext] USBToolBox](https://github.com/USBToolBox/kext)

## Credits

- [Apple](https://apple.com)
- [Acidanthera](https://github.com/acidanthera/OpenCorePkg)
- [Dortania](https://dortania.github.io/OpenCore-Install-Guide/)
- Guys who make kexts
