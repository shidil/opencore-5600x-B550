# B550 Desktop Ryzentosh (R5 5600x)

OpenCore bootloader config files for my workstation hackintosh.

`RX 6800` support arrived on Big Sur 11.4

## System Information

| Name     |                     Model |
| :------- | ------------------------: |
| CPU      |             Ryzen 5 5600x |
| GPU      |               AMD RX 6800 |
| SSD      | Samsung 970 Evo Plus NVMe |
| WiFi     |  TP-Link T9E (BCM driver) |
| Board    |            MSI B550 A-Pro |
| Ethernet |      RTL8111H Gigabit LAN |

- OpenCore: v0.6.8
- MacOS: v11.4 BigSur
- OpenCanopy theme: <https://github.com/tekteq/opencanopy-minimal-theme>

## Guide

<https://dortania.github.io/OpenCore-Install-Guide/prerequisites.html>
<https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html>

### SMBIOS

Selected: `MacPro7,1`

Don't forget to change device uuid, board serials and network mac address
Go to <https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#platforminfo> For information on setting up SMBIOS platform info

## Kexts Used

| Package                  | Version |
| :----------------------- | ------: |
| AppleALC                 |   1.5.9 |
| Lilu                     |   1.5.2 |
| VirtualSMC               |   1.2.2 |
| AirportBcrmFixup         |   2.1.2 |
| RealtekRTL8111           |   2.4.0 |
| NVMeFix                  |   1.0.7 |
| AppleMCEReporterDisabler |   1.2.0 |
| RestrictEvents           |   1.0.0 |

## What works

- [x] Graphics
- [x] iServices
- [x] USB
- [x] WiFi
- [x] Bluetooth
- [x] Sleep
- [x] Audio
- [x] iOS Simulator

## What's not working

- Yet to find out, everything seems to be working fine. Ethernet is not tested.


## Pre Install

- Update SMBIOS and MAC address
  
## Post Install

- Upgrade OpenCore versions
  