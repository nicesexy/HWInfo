Devices with poor Linux-compatibility
=====================================

This is a project to find PCI/USB devices with poor Linux-compatibility based on the hwinfo
reports (https://github.com/openSUSE/hwinfo) collected by Linux users at https://linux-hardware.org.

In the scope of this project, the device is considered poorly supported by Linux if driver
is not found for this device in at least one user probe on any Linux distribution.

You can find appropriate hwinfo report in this repository by a probe ID as follows:

    find . -name {PROBE ID}

Everyone can contribute to this repository by uploading probes of their computers
by the hw-probe tool (https://github.com/linuxhw/hw-probe):

    sudo hw-probe -all -upload

Total reports: 29202.

Contents
--------

1. [ About ](#about)
2. [ PCI Devices ](#pci-devices)
   * [ Bluetooth ](#bluetooth-pci)
   * [ Card reader ](#card-reader-pci)
   * [ Communication controller ](#communication-controller-pci)
   * [ Flash memory ](#flash-memory-pci)
   * [ Graphics card ](#graphics-card-pci)
   * [ Modem ](#modem-pci)
   * [ Multimedia controller ](#multimedia-controller-pci)
   * [ Net/ethernet ](#netethernet-pci)
   * [ Net/wireless ](#netwireless-pci)
   * [ Network ](#network-pci)
   * [ Sound ](#sound-pci)
   * [ Storage ](#storage-pci)
   * [ Storage/ata ](#storageata-pci)
   * [ Storage/raid ](#storageraid-pci)
   * [ System peripheral ](#system-peripheral-pci)
   * [ Tv card ](#tv-card-pci)
   * [ Usb controller ](#usb-controller-pci)
3. [ USB Devices ](#usb-devices)
   * [ Audio ](#audio-usb)
   * [ Bluetooth ](#bluetooth-usb)
   * [ Camera ](#camera-usb)
   * [ Card reader ](#card-reader-usb)
   * [ Chipcard ](#chipcard-usb)
   * [ Converter ](#converter-usb)
   * [ Disk ](#disk-usb)
   * [ Dvb card ](#dvb-card-usb)
   * [ Fingerprint reader ](#fingerprint-reader-usb)
   * [ Hardware key ](#hardware-key-usb)
   * [ Hasp ](#hasp-usb)
   * [ Hub ](#hub-usb)
   * [ Human interface ](#human-interface-usb)
   * [ Imaging ](#imaging-usb)
   * [ Input/keyboard ](#inputkeyboard-usb)
   * [ Input/mouse ](#inputmouse-usb)
   * [ Modem ](#modem-usb)
   * [ Net/wimax ](#netwimax-usb)
   * [ Net/wireless ](#netwireless-usb)
   * [ Network ](#network-usb)
   * [ Tv card ](#tv-card-usb)
   * [ Video ](#video-usb)
   * [ Wireless ](#wireless-usb)

About
-----

The structure of the repository is the following:

    {COMPUTER TYPE}/{VENDOR}/{MODEL PREFIX}/{MODEL}/{HWID}/{OS}/{KERNEL}/{ARCH}/{PROBE ID}

    ( e.g. Notebook/Dell/XPS/XPS L421X/D7DA07727B83/ROSA-2014.1/3.14.22-NRJ-LAPTOP-3ROSA/X86_64/F74F6103A1 )

PCI Devices
-----------

Non-100% value in the 'Missed' column indicates that the driver for a device is available
in the latest kernel versions. You can find corresponding hwinfo reports for listed devices
by a probe ID.

Missed — percentage of probes with missed driver for the device,
Linux  — the minimum Linux kernel version in which the driver was found,
Probe  — latest probe ID with missed driver for the device.

### Bluetooth (PCI)

6 out of 6 (100%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1814:3298 | 103c:18ec | Ralink          | RT3290 Bluetooth         | 100%   |          | 97E765D4F6 |
| 1814:3298 | 105b:e056 | Ralink          | RT3290 Bluetooth         | 100%   |          | A5ABFDA33A |
| 1814:3298 | 1814:3298 | Ralink          | RT3290 Bluetooth         | 100%   |          | FE9255E7F3 |
| 1814:3298 | 1a3b:2787 | Ralink          | RT3290 Bluetooth         | 100%   |          | 0E1770A053 |
| 1814:3298 | 1a3b:2987 | Ralink          | RT3290 Bluetooth         | 100%   |          | 8D13B8BFE3 |
| 1814:3298 | 1a3b:2f87 | Ralink          | RT3290 Bluetooth         | 100%   |          | 31B34A5C64 |

### Card reader (PCI)

7 out of 351 (1.99%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 10ec:5227 | 1179:0001 | Realtek Semi... | RTS5227 PCI Express C... | 100%   |          | 550460AAAC |
| 10ec:522a | 103c:806e | Realtek Semi... | RTS522A PCI Express C... | 100%   |          | 62A9EF950E |
| 10ec:522a | 103c:80a4 | Realtek Semi... | RTS522A PCI Express C... | 33.3%  | 4.9.60   | B01FB51118 |
| 10ec:522a | 103c:820c | Realtek Semi... | RTS522A PCI Express C... | 33.3%  | 4.9.20   | FAE1CD27F3 |
| 10ec:522a | 17aa:5113 | Realtek Semi... | RTS522A PCI Express C... | 100%   |          | 32F7318757 |
| 10ec:5287 | 1025:0866 | Realtek Semi... | RTL8411B PCI Express ... | 1.9%   | 3.14.25  | 798177A8A9 |
| 1aea:6601 | 1179:f900 | Alcor Micro     | AU6601 PCI-E Flash ca... | 100%   |          | 43A9D7922A |

### Communication controller (PCI)

98 out of 1214 (8.07%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 04f1:2f20 | 04f1:200c |                 | Communication controller | 100%   |          | 6759172767 |
| 104c:8035 | 103c:0944 | Texas Instru... | PCI6411/6421/6611/662... | 100%   |          | B174748BA7 |
| 104c:8038 | 1028:0182 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | F53A4FB405 |
| 104c:8038 | 1028:0186 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | D3C59F7F90 |
| 104c:8038 | 1028:0187 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | 358447EB4E |
| 104c:803d | 103c:309f | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 5BE41E5F47 |
| 104c:803d | 103c:30a3 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | E5523A66D5 |
| 104c:803d | 103c:30ac | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 2091D320DC |
| 104c:803d | 103c:30b1 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | D4DC67EA5D |
| 104c:803d | 1071:8212 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 01F778FE4E |
| 11c1:0480 | 1668:0500 | LSI             | Venus Modem (V90, 56K... | 50%    | 3.14.22  | 0A61436F40 |
| 11c1:048c | 11c1:044c | LSI             | V.92 56K WinModem        | 100%   |          | BBA3DE40E2 |
| 11c1:0620 | 11c1:0620 | LSI             | Lucent V.92 Data/Fax ... | 100%   |          | D301F3A17A |
| 11c1:0630 | 11c1:0630 | LSI             | Agere Communication c... | 100%   |          | 36661C8538 |
| 11c1:0630 | 11c1:0631 | LSI             | Agere Communication c... | 100%   |          | A496E46CB4 |
| 13f6:0211 | 13f6:0211 | C-Media Elec... | CM8738                   | 100%   |          | F54FCFF2DE |
| 14f1:10b6 | 14f1:10b6 | Conexant Sys... | CX06834-11 HCF V.92 5... | 100%   |          | DB02CE55DC |
| 14f1:2013 | 13e0:0212 | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 3ED411EF5C |
| 14f1:2702 | 14f1:2007 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | 83629CDF01 |
| 14f1:2f00 | 14f1:2003 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | AF474622B9 |
| 14f1:2f00 | 14f1:2004 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 212AC6575E |
| 14f1:2f00 | 187e:3409 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 862C8CAD94 |
| 14f1:2f12 | 16ec:2016 | Conexant Sys... | Conexant Communicatio... | 100%   |          | 3ADDAB1A1D |
| 14f1:2f20 | 14f1:200c | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 97BAE2C4D6 |
| 14f1:2f20 | 14f1:200f | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | D5B3BF7481 |
| 14f1:2f30 | 14f1:2051 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 7E932C8DF9 |
| 14f1:2f30 | 14f1:20d5 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | F37C9C9E3F |
| 14f1:2f40 | 14f1:2000 | Conexant Sys... | Conexant Communicatio... | 100%   |          | 1F97EF92E1 |
| 14f1:2f81 | 14f1:0000 | Conexant Sys... | Conexant Communicatio... | 100%   |          | 4C1091E630 |
| 1fd4:1999 | 1fd4:0101 | SUNIX           | Multiport serial cont... | 100%   |          | 2649527FFD |
| 8086:1c3a | 1043:844d | Intel           | 6 Series/C200 Series ... | 0.1%   | 3.0.38   | 1678EE56C3 |
| 8086:1c3a | 17aa:3975 | Intel           | 6 Series/C200 Series ... | 0.9%   | 3.10.34  | 2239D316E8 |
| 8086:1d3a | 15d9:0628 | Intel           | C600/X79 series chips... | 100%   |          | 99E743CA9E |
| 8086:1d3b | 15d9:0628 | Intel           | C600/X79 series chips... | 100%   |          | 99E743CA9E |
| 8086:1d3b | 8086:357e | Intel           | C600/X79 series chips... | 100%   |          | DF1B417E9A |
| 8086:3b64 | 1043:1c77 | Intel           | 5 Series/3400 Series ... | 1.2%   | 3.14.25  | 7FDEE4E7BB |
| 8086:5a9a | 8086:7270 | Intel           | Celeron N3350/Pentium... | 25%    | 4.9.60   | 8ADD68C95A |
| 8086:5a9c | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9c | 1043:8738 | Intel           | Communication controller | 100%   |          | 82BDD3F39F |
| 8086:5a9c | 17aa:3802 | Intel           | Communication controller | 100%   |          | B02B76DC46 |
| 8086:5a9c | 17aa:3809 | Intel           | Communication controller | 100%   |          | 226C39CA6E |
| 8086:5a9e | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9e | 1043:8738 | Intel           | Communication controller | 100%   |          | 82BDD3F39F |
| 8086:5a9e | 17aa:3802 | Intel           | Communication controller | 100%   |          | B02B76DC46 |
| 8086:5a9e | 17aa:380a | Intel           | Communication controller | 100%   |          | 226C39CA6E |
| 8086:8c3a | 1028:0620 | Intel           | 8 Series/C220 Series ... | 100%   |          | F801FAB1AD |
| 8086:8c3a | 1043:8534 | Intel           | 8 Series/C220 Series ... | 0.3%   | 3.14.25  | 4712036FF4 |
| 8086:8c3a | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 100%   |          | DB25C87154 |
| 8086:8c3b | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 100%   |          | DB25C87154 |
| 8086:8cba | 1458:1c3a | Intel           | 9 Series Chipset Fami... | 2%     | 3.14.22  | 5A77B72FE5 |
| 8086:8d3a | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3a | 8086:7270 | Intel           | C610/X99 series chips... | 50%    | 4.14.18  | EDE05678EF |
| 8086:8d3b | 15d9:0821 | Intel           | C610/X99 series chips... | 100%   |          | 37AEC1E068 |
| 8086:8d3b | 15d9:0831 | Intel           | C610/X99 series chips... | 100%   |          | F0EB4348F0 |
| 8086:8d3b | 15d9:0835 | Intel           | C610/X99 series chips... | 100%   |          | 7479576DA8 |
| 8086:8d3b | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3b | 8086:7270 | Intel           | C610/X99 series chips... | 100%   |          | BF0A7F04B4 |
| 8086:9d3a | 1025:1094 | Intel           | Sunrise Point-LP CSME... | 25%    | 4.9.9    | E7D6077756 |
| 8086:9d3a | 1028:06de | Intel           | Sunrise Point-LP CSME... | 100%   |          | AE7AD1E7D9 |
| 8086:9d3a | 1028:06fd | Intel           | Sunrise Point-LP CSME... | 100%   |          | 98D787F0D4 |
| 8086:9d3a | 1028:0782 | Intel           | Sunrise Point-LP CSME... | 100%   |          | 49389100FC |
| 8086:9d3a | 103c:8079 | Intel           | Sunrise Point-LP CSME... | 62.5%  | 4.4.1    | F1A8589F00 |
| 8086:9d3a | 103c:80a4 | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.9.60   | B01FB51118 |
| 8086:9d3a | 103c:80ff | Intel           | Sunrise Point-LP CSME... | 85.7%  | 4.7.2    | B7B039F46E |
| 8086:9d3a | 103c:8100 | Intel           | Sunrise Point-LP CSME... | 100%   |          | 2B56F34E21 |
| 8086:9d3a | 103c:8101 | Intel           | Sunrise Point-LP CSME... | 66.7%  | 4.9.60   | BC496704F4 |
| 8086:9d3a | 103c:820c | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.9.20   | FAE1CD27F3 |
| 8086:9d3a | 1043:1ccd | Intel           | Sunrise Point-LP CSME... | 50%    | 4.9.20   | A4B26975E9 |
| 8086:9d3a | 1179:f820 | Intel           | Sunrise Point-LP CSME... | 100%   |          | B781D8419A |
| 8086:9d3a | 17aa:3801 | Intel           | Sunrise Point-LP CSME... | 7.7%   | 4.9.9    | 412EAC636F |
| 8086:9d3a | 17aa:3808 | Intel           | Sunrise Point-LP CSME... | 16.7%  | 4.9.20   | 9B61CC7F7F |
| 8086:9d3a | 17aa:380c | Intel           | Sunrise Point-LP CSME... | 100%   |          | C3352134E9 |
| 8086:9d3a | 17aa:3819 | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.9.0    | 18379EBD5C |
| 8086:9d3a | 17aa:382d | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.9.60   | 65FE9A36B5 |
| 8086:9d3a | 17aa:5048 | Intel           | Sunrise Point-LP CSME... | 100%   |          | 842B139FE7 |
| 8086:a13a | 1019:9bc9 | Intel           | Sunrise Point-H CSME ... | 100%   |          | 744A3F2E54 |
| 8086:a13a | 1019:9c56 | Intel           | Sunrise Point-H CSME ... | 100%   |          | 093E3BB0DE |
| 8086:a13a | 1028:06de | Intel           | Sunrise Point-H CSME ... | 100%   |          | BC4C6EBBA7 |
| 8086:a13a | 1028:06f7 | Intel           | Sunrise Point-H CSME ... | 100%   |          | E2D11AD2AC |
| 8086:a13a | 1043:1080 | Intel           | Sunrise Point-H CSME ... | 100%   |          | 5B1076EA3C |
| 8086:a13a | 1043:1d6d | Intel           | Sunrise Point-H CSME ... | 100%   |          | 9D6C0DD372 |
| 8086:a13a | 1043:8694 | Intel           | Sunrise Point-H CSME ... | 21.3%  | 4.4.0    | A91734714E |
| 8086:a13a | 1458:1c3a | Intel           | Sunrise Point-H CSME ... | 36.8%  | 4.4.16   | 53E6A4F263 |
| 8086:a13a | 1462:116e | Intel           | Sunrise Point-H CSME ... | 100%   |          | 1C47BC90E4 |
| 8086:a13a | 1462:1190 | Intel           | Sunrise Point-H CSME ... | 16.7%  | 4.9.9    | 2B70AAB06F |
| 8086:a13a | 1462:7970 | Intel           | Sunrise Point-H CSME ... | 20%    | 4.9.20   | AC10EFBB42 |
| 8086:a13a | 1462:7982 | Intel           | Sunrise Point-H CSME ... | 100%   |          | AE97650E7C |
| 8086:a13a | 1462:7995 | Intel           | Sunrise Point-H CSME ... | 100%   |          | 7D25E0B2DD |
| 8086:a13a | 1462:7996 | Intel           | Sunrise Point-H CSME ... | 37.5%  | 4.9.20   | A4FFA622A4 |
| 8086:a13a | 17aa:3802 | Intel           | Sunrise Point-H CSME ... | 33.3%  | 4.4.16   | 25576A8571 |
| 8086:a13a | 1849:a13a | Intel           | Sunrise Point-H CSME ... | 14.3%  | 4.3.3    | 9869646781 |
| 8086:a13a | 8086:1999 | Intel           | Sunrise Point-H CSME ... | 50%    | 4.9.20   | 13B41B547A |
| 8086:a13b | 8086:1999 | Intel           | Sunrise Point-H CSME ... | 100%   |          | 13B41B547A |
| 8086:a1be | 8086:7270 | Intel           | Lewisburg CSME: HECI #3  | 100%   |          | F8D0599716 |
| 8086:a2ba | 1458:1c3a | Intel           | 200 Series PCH CSME H... | 4.5%   | 4.9.9    | 6126E55D1A |
| 8086:a2ba | 1462:7a71 | Intel           | 200 Series PCH CSME H... | 100%   |          | 309262E3D6 |
| 8086:a360 | 1458:1c3a | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 28D5F5C509 |
| 9710:9900 | a000:2000 | MosChip Semi... | NetMos Communication ... | 100%   |          | 7D609B3954 |

### Flash memory (PCI)

23 out of 39 (58.97%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1524:0520 | 1025:007a | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | E4219525B9 |
| 1524:0520 | 1025:0090 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | EBB380841E |
| 1524:0520 | 1025:009f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 2FFCA69E4A |
| 1524:0520 | 1025:010f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 7344AA6577 |
| 1524:0530 | 1025:007a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | E4219525B9 |
| 1524:0530 | 1025:0090 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | EBB380841E |
| 1524:0530 | 1025:009f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 2FFCA69E4A |
| 1524:0530 | 1025:010f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 7344AA6577 |
| 1524:0530 | 14c0:0020 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 09E34C2375 |
| 1524:0530 | 1734:10c1 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | A329D1DF25 |
| 1524:0530 | 1734:10d7 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | CA3AC06D30 |
| 1524:0720 | 1025:011b | ENE Technology  | Memory Stick Card Rea... | 100%   |          | B614684231 |
| 1524:0720 | 1025:012a | ENE Technology  | Memory Stick Card Rea... | 100%   |          | C95503E7D2 |
| 1524:0720 | 1025:012e | ENE Technology  | Memory Stick Card Rea... | 100%   |          | B8EED87A42 |
| 1524:0720 | 1462:2fb3 | ENE Technology  | Memory Stick Card Rea... | 100%   |          | D6A996DA64 |
| 1524:0720 | 1462:2fbd | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 5DD14F9164 |
| 1524:0730 | 1025:011b | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | B614684231 |
| 1524:0730 | 1025:012a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C95503E7D2 |
| 1524:0730 | 1025:012e | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | B8EED87A42 |
| 1524:0730 | 1462:2fb3 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | D6A996DA64 |
| 1524:0730 | 1462:2fbd | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 5DD14F9164 |
| 1524:0730 | 1558:0664 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 51E2E84C28 |
| 1524:0730 | 1558:0668 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 41C9811E8B |

### Graphics card (PCI)

80 out of 6366 (1.26%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:15dd | 1043:876b | AMD/ATI         | Raven Ridge [Radeon V... | 100%   |          | A04FA68080 |
| 1002:5b70 | 0000:0001 | ATI Technolo... | RV370 [Radeon X300 SE]   | 100%   |          | 8E9A9E1E93 |
| 1002:67df | 1002:0b37 | AMD/ATI         | Ellesmere [Polaris10]    | 100%   |          | 5CC9EEEBFE |
| 1002:67df | 1043:04b0 | AMD/ATI         | Ellesmere [Polaris10]    | 100%   |          | 713B99FFC5 |
| 1002:67ef | 1043:04b2 | AMD/ATI         | Baffin [Radeon RX 460... | 50%    | 4.9.20   | 0E0A089DEF |
| 1002:67ef | 174b:e348 | AMD/ATI         | Baffin [Radeon RX 460... | 20%    | 4.9.20   | 72DD80DA38 |
| 1002:67ff | 1458:22fb | AMD/ATI         | Baffin [Radeon RX 560]   | 50%    | 4.9.60   | BE6A2708EB |
| 1002:68e4 | 1043:1c92 | AMD/ATI         | Robson CE [Radeon HD ... | 4.5%   | 3.14.44  | 7FDEE4E7BB |
| 1002:6900 | 103c:2269 | AMD/ATI         | Topaz XT [Radeon R7 M... | 25%    | 4.9.20   | 912D4C6523 |
| 1002:6900 | 103c:226b | AMD/ATI         | Topaz XT [Radeon R7 M... | 50%    | 3.14.53  | 1A71B0CAF6 |
| 1002:6900 | 103c:22c8 | AMD/ATI         | Topaz XT [Radeon R7 M... | 66.7%  | 4.9.41   | 91B2B00C8A |
| 1002:6900 | 103c:8229 | AMD/ATI         | Topaz XT [Radeon R7 M... | 66.7%  | 4.10.0   | 1E1F16D2E9 |
| 1002:6938 | 1043:04f5 | AMD/ATI         | Tonga XT / Amethyst X... | 12.5%  | 4.1.22   | 0E1E35C6E2 |
| 1002:6939 | 148c:9380 | AMD/ATI         | Tonga PRO [Radeon R9 ... | 50%    | 4.9.20   | EC8854521E |
| 1002:6939 | 1682:9380 | AMD/ATI         | Tonga PRO [Radeon R9 ... | 100%   |          | A3F6229CAA |
| 1002:6939 | 174b:e308 | AMD/ATI         | Tonga PRO [Radeon R9 ... | 9.1%   | 4.1.16   | 77EF398855 |
| 1002:699f | 1458:22f2 | AMD/ATI         | Lexa PRO [Radeon RX 550] | 100%   |          | 96683C37E1 |
| 1002:699f | 1462:8a90 | AMD/ATI         | Lexa PRO [Radeon RX 550] | 100%   |          | 100AA405E8 |
| 1002:9851 | 1025:088c | AMD/ATI         | Mullins [Radeon R4/R5... | 50%    | 4.0.4    | D0E8E1E8D9 |
| 1002:9851 | 103c:2269 | AMD/ATI         | Mullins [Radeon R4/R5... | 25%    | 4.9.20   | 912D4C6523 |
| 1002:9851 | 103c:226b | AMD/ATI         | Mullins [Radeon R4/R5... | 16.7%  | 3.14.53  | 8016AF5575 |
| 1002:9851 | 103c:22c2 | AMD/ATI         | Mullins [Radeon R4/R5... | 66.7%  | 4.1.8    | 4989738540 |
| 1002:9851 | 103c:22cd | AMD/ATI         | Mullins [Radeon R4/R5... | 100%   |          | 46004F2E8E |
| 1002:9851 | 17aa:3801 | AMD/ATI         | Mullins [Radeon R4/R5... | 6.7%   | 4.1.15   | A30A019453 |
| 1002:9851 | 17aa:3819 | AMD/ATI         | Mullins [Radeon R4/R5... | 18.2%  | 4.1.15   | 6FF4E5324B |
| 1002:9853 | 17aa:3800 | AMD/ATI         | Mullins [Radeon APU E... | 11.1%  | 3.14.44  | 23A8BF660D |
| 1002:9874 | 103c:80b6 | AMD/ATI         | Carrizo                  | 100%   |          | C7EEDACBF5 |
| 1002:9874 | 17aa:5113 | AMD/ATI         | Carrizo                  | 100%   |          | 32F7318757 |
| 1002:98e4 | 17aa:39f9 | AMD/ATI         | Stoney [Radeon R2/R3/... | 25%    | 4.9.20   | C23D0EF968 |
| 1022:6840 |           | AMD             | VGA compatible contro... | 100%   |          | 065591BE36 |
| 1023:2100 | 1179:0001 | Trident Micr... | CyberBlade XP4m32        | 100%   |          | F39BB50139 |
| 102b:0522 | 8086:0103 | Matrox Elect... | MGA G200e [Pilot] Ser... | 66.7%  | 4.1.38   | DF1B417E9A |
| 102b:0532 | 1028:0235 | Matrox Elect... | MGA G200eW WPCM450       | 100%   |          | 186F3C15DD |
| 102b:0532 | 15d9:0006 | Matrox Elect... | MGA G200eW WPCM450       | 87.5%  | 4.1.15   | C60718AEF4 |
| 102b:0532 | 15d9:0009 | Matrox Elect... | MGA G200eW WPCM450       | 100%   |          | BB7B1076F6 |
| 102b:0532 | 15d9:0624 | Matrox Elect... | MGA G200eW WPCM450       | 25%    | 3.10.34  | 069356D316 |
| 102b:0532 | 15d9:0628 | Matrox Elect... | MGA G200eW WPCM450       | 100%   |          | 99E743CA9E |
| 102b:0533 | 103c:3381 | Matrox Elect... | MGA G200EH               | 80%    | 3.14.25  | 2D74AD691D |
| 102b:0534 | 1014:0405 | Matrox Elect... | G200eR2                  | 100%   |          | D7CBC31CEE |
| 1033:0165 | 1461:6510 | NEC             | Multimedia video cont... | 100%   |          | 106570BBC3 |
| 1033:0165 | 1461:652c | NEC             | Multimedia video cont... | 100%   |          | 9D61E4EA0B |
| 1039:6351 | 1019:5050 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | CA495AA6C4 |
| 1039:6351 | 1019:5055 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | 7EE2739156 |
| 1039:6351 | 1043:1812 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | 9DA40A383A |
| 1039:6351 | 1043:19e2 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | 22B272C2D6 |
| 1039:6351 | 1043:82c9 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | 62B1AE15F1 |
| 1039:6351 | 1558:0804 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | 9CF9B915F2 |
| 1039:6351 | 1631:c10b | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | B0517198DD |
| 1039:6351 | 1734:1110 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | C34E5866A6 |
| 1039:6351 | 1734:1125 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | DF41C6F9E2 |
| 1039:6351 | 17ff:0594 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | F248142F16 |
| 1039:6351 | 1b0a:0007 | Silicon Inte... | 771/671 PCIE VGA Disp... | 100%   |          | E60EF0934C |
| 104d:8087 | 104d:80ed | Sony            | Multimedia video cont... | 100%   |          | 72A578315E |
| 14f1:5851 |           | Conexant Sys... | Conexant Multimedia v... | 100%   |          | 88FFC14224 |
| 1797:6804 |           | Intersil Tec... | Multimedia video cont... | 100%   |          | B2C845B843 |
| 1797:6804 | 1797:6804 | Intersil Tec... | Multimedia video cont... | 100%   |          | B2C845B843 |
| 1a03:2000 | 15d9:0884 | ASPEED Techn... | ASPEED Graphics Family   | 100%   |          | 9B891A8CD9 |
| 1a03:2000 | 1a03:2000 | ASPEED Techn... | ASPEED Graphics Family   | 66.7%  | 4.1.34   | EDE05678EF |
| 1a0a:6200 | 1461:6201 |                 | Multimedia video cont... | 100%   |          | 3D855922B8 |
| 1a0a:6202 | 1461:6201 |                 | Multimedia video cont... | 100%   |          | 069D08FB9E |
| 1a0a:6202 | 1461:6205 |                 | Multimedia video cont... | 100%   |          | DCE3E0D766 |
| 1a0a:6202 | 1461:6216 |                 | Multimedia video cont... | 100%   |          | C7E0EC2ADD |
| 1a0a:6202 | 1461:621a |                 | Multimedia video cont... | 100%   |          | C7A8CDAFE8 |
| 1ade:3038 | 4254:5580 | Spin Master     | Multimedia video cont... | 25%    | 4.1.4    | C4768A03B3 |
| 5254:0820 |           |                 | Multimedia video cont... | 100%   |          | E60DBB1D7C |
| 8086:0f31 | 1025:0936 | Intel           | ValleyView Gen7          | 100%   |          | 1718CF1D36 |
| 8086:1616 | 1028:062b | Intel           | Broadwell-U Integrate... | 100%   |          | 0A99E4D896 |
| 8086:1916 | 17aa:382c | Intel           | Skylake GT2 [HD Graph... | 50%    | 4.9.0    | 18379EBD5C |
| 8086:191b | 1043:1080 | Intel           | VGA compatible contro... | 100%   |          | 5B1076EA3C |
| 8086:22b1 | 1025:1012 | Intel           | Atom/Celeron/Pentium ... | 12.5%  | 4.9.20   | 16D1C62342 |
| 8086:22b1 | 1043:10c0 | Intel           | Atom/Celeron/Pentium ... | 7.7%   | 4.1.25   | E6AFAB9B56 |
| 8086:22b1 | 1043:1d5d | Intel           | Atom/Celeron/Pentium ... | 14.3%  | 4.9.20   | 27173939AA |
| 8086:22b1 | 1558:0945 | Intel           | Atom/Celeron/Pentium ... | 8.3%   | 4.1.15   | BDAF59B6EB |
| 8086:22b1 | 8086:2060 | Intel           | Atom/Celeron/Pentium ... | 14.3%  | 4.1.15   | 5738D326F6 |
| 8086:3e91 | 1043:8694 | Intel           | VGA compatible contro... | 100%   |          | DA54361164 |
| 8086:5912 | 1043:8694 | Intel           | HD Graphics 630          | 4.2%   | 4.4.49   | B0DE2CBA6A |
| 8086:5912 | 1458:d000 | Intel           | VGA compatible contro... | 16.7%  | 4.9.60   | 6126E55D1A |
| 8086:5916 | 1028:0782 | Intel           | VGA compatible contro... | 100%   |          | 49389100FC |
| 8086:5916 | 17aa:39f1 | Intel           | VGA compatible contro... | 33.3%  | 4.9.60   | 65FE9A36B5 |
| 8086:a011 | 1462:104e | Intel           | Atom Processor D4xx/D... | 25%    | 4.1.15   | 5F15F028A8 |

### Modem (PCI)

10 out of 63 (15.87%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1057:3052 | 1057:3020 | Motorola        | SM56 Data Fax Modem      | 100%   |          | EDF7BDEF30 |
| 10b9:5457 | 103c:0850 | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 4E9D284D9C |
| 11c1:0440 | 11c1:0440 | LSI             | 56k WinModem             | 100%   |          | 6B2E5020C2 |
| 11c1:0449 | 1468:0410 | LSI             | L56xM+S [Mars-2] WinM... | 100%   |          | A8A13EFBA0 |
| 11c1:044c | 11c1:044c | LSI             | LT WinModem              | 100%   |          | 0530399CDF |
| 11c1:044e | 11c1:044e | LSI             | LT WinModem              | 100%   |          | 6203763CC5 |
| 11c1:044e | 1235:044e | LSI             | LT WinModem              | 100%   |          | 3D74179CB7 |
| 1543:3052 | 1543:3000 | SILICON Labo... | Intel 537 [Winmodem]     | 100%   |          | 75C969D54B |
| 2003:8800 | 16ef:2800 | Smart Link      | LM-I56N                  | 100%   |          | 8B4AE6CF41 |
| 8086:1040 | 8086:1000 | Intel           | 536EP Data Fax Modem     | 100%   |          | D561042A58 |

### Multimedia controller (PCI)

56 out of 67 (83.58%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:4d51 | 1002:b041 | AMD/ATI         | Multimedia controller    | 100%   |          | 2CF316774E |
| 1002:ac12 | 1002:b539 | AMD/ATI         | Theater HD T507 (DVB-... | 100%   |          | DD5E0979B0 |
| 1002:ac12 | 12ab:0003 | AMD/ATI         | Theater HD T507 (DVB-... | 100%   |          | 60AE7E3358 |
| 1002:ad18 | 1682:ad18 | AMD/ATI         | Multimedia controller    | 100%   |          | 3108FE53D3 |
| 109e:0878 |           | Brooktree       | Bt878 Audio Capture      | 100%   |          | ECE7B322E7 |
| 109e:0878 | 1047:f331 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 444FFBC8A6 |
| 109e:0878 | 107d:6609 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 2B35A8BCF0 |
| 109e:0878 | 1461:0001 | Brooktree       | Bt878 Audio Capture      | 100%   |          | E8072B6F3A |
| 109e:0878 | 1461:0002 | Brooktree       | Bt878 Audio Capture      | 100%   |          | A22609B54B |
| 109e:0878 | 1461:0004 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 660B28DD52 |
| 1131:7160 | 1461:0855 | Philips Semi... | SAA7160                  | 100%   |          | E507592DE8 |
| 1131:7160 | 1461:0a55 | Philips Semi... | SAA7160                  | 100%   |          | 99DDBBF195 |
| 1131:7160 | 1461:1055 | Philips Semi... | SAA7160                  | 100%   |          | 9E921922BA |
| 1131:7160 | 1461:1455 | Philips Semi... | SAA7160                  | 100%   |          | C785DD2710 |
| 1131:7160 | 1461:2655 | Philips Semi... | SAA7160                  | 100%   |          | A74B989748 |
| 1131:7160 | 16be:0034 | Philips Semi... | SAA7160                  | 100%   |          | 2B8D93B7EC |
| 1131:7160 | 1ae4:0700 | Philips Semi... | SAA7160                  | 100%   |          | DA3F12C69C |
| 1131:7160 | 6281:0001 | Philips Semi... | SAA7160                  | 16.7%  | 4.9.76   | AA733E4B02 |
| 1131:7162 | 11bd:0100 | Philips Semi... | SAA7162                  | 100%   |          | EF8A743A1E |
| 1131:7162 | 11bd:0101 | Philips Semi... | SAA7162                  | 100%   |          | 003EB89135 |
| 1131:7231 | 12ab:0762 | Philips Semi... | SAA7231                  | 100%   |          | 95E9C97144 |
| 1131:7231 | 12ab:0763 | Philips Semi... | SAA7231                  | 100%   |          | FFFD5B7F79 |
| 1131:7231 | 1461:0b0f | Philips Semi... | SAA7231                  | 100%   |          | 791CA50070 |
| 1131:7231 | 1461:110f | Philips Semi... | SAA7231                  | 100%   |          | 90DFBFB6FA |
| 1131:7231 | 1461:1400 | Philips Semi... | SAA7231                  | 100%   |          | 44A4BF3536 |
| 1131:7231 | 1461:2a0f | Philips Semi... | SAA7231                  | 100%   |          | 25DFBA352F |
| 1131:7231 | 1461:2b0f | Philips Semi... | SAA7231                  | 100%   |          | F92CB57F54 |
| 1131:7231 | 1461:7983 | Philips Semi... | SAA7231                  | 100%   |          | 6F56951660 |
| 1131:7231 | 16be:0008 | Philips Semi... | SAA7231                  | 100%   |          | F475557A99 |
| 1131:7231 | 5ace:8000 | Philips Semi... | SAA7231                  | 100%   |          | A558A93779 |
| 1131:7231 | 5ace:8150 | Philips Semi... | SAA7231                  | 100%   |          | 8603D5BDF5 |
| 1131:7231 | 5ace:8201 | Philips Semi... | SAA7231                  | 100%   |          | 11F9FB0623 |
| 11bd:bede | 11bd:0022 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | 03BC1C611D |
| 11bd:bede | 11bd:0023 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | 43E1A4811A |
| 14e4:1570 | 14e4:1570 | Broadcom Lim... | 720p FaceTime HD Camera  | 100%   |          | A1A5EFDC18 |
| 14e4:1612 | 14e4:2612 | Broadcom        | BCM70012 Video Decode... | 100%   |          | 71EDB71D27 |
| 14e4:1615 | 105b:0d77 | Broadcom        | BCM70015 Video Decode... | 100%   |          | B036D312E6 |
| 14e4:1615 | 14e4:1615 | Broadcom        | BCM70015 Video Decode... | 100%   |          | 2606C71952 |
| 14f1:8804 | 0070:9202 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | DFF9C11E07 |
| 14f1:8804 | 1822:0023 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | AB36F565A4 |
| 1745:2100 | 1043:48b0 | ViXS Systems    | XCode 2100 Series        | 100%   |          | AD1D92439F |
| 1797:6805 |           | Intersil Tec... | Multimedia controller    | 100%   |          | B2C845B843 |
| 1797:6805 | 1797:6804 | Intersil Tec... | Multimedia controller    | 100%   |          | B2C845B843 |
| 1822:4e35 | 1822:0048 | Twinhan Tech... | Mantis DTV PCI Bridge... | 100%   |          | CB1A0D9CDD |
| 8086:0f38 | 8086:0f31 | Intel           | Atom Processor Z36xxx... | 85.7%  | 4.12.4   | A419E65F55 |
| 8086:0f38 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 100%   |          | E277646CEF |
| 8086:1919 | 8086:1919 | Intel           | Skylake Imaging Unit     | 100%   |          | 23C4F883A7 |
| 8086:1919 | 8086:2015 | Intel           | Skylake Imaging Unit     | 100%   |          | 02E23B6024 |
| 8086:22b8 | 1025:106e | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 425D589D65 |
| 8086:22b8 | 103c:827c | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 57910E3D67 |
| 8086:22b8 | 1043:13a0 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | C508886F10 |
| 8086:22b8 | 1043:1400 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 90B9B380A5 |
| 8086:22b8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 037FFBE89A |
| 8086:5a88 |           | Intel           | Celeron N3350/Pentium... | 100%   |          | 8ADD68C95A |
| 8086:9d32 | 8086:9d32 | Intel           | Multimedia controller    | 100%   |          | 23C4F883A7 |
| dd01:0006 | dd01:0022 | Digital Devices | Cine V7                  | 100%   |          | FCF4AFE5C6 |

### Net/ethernet (PCI)

7 out of 2171 (0.32%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 000c:0000 | 1043:83a3 |                 | Ethernet controller      | 100%   |          | B5189C3BF2 |
| 10ec:0139 | 10bd:0320 | Realtek Semi... | RTL-8139/8139C/8139C+... | 100%   |          | 305C35F50C |
| 10ec:8136 | 1028:0555 | Realtek Semi... | RTL8101/2/6E PCI Expr... | 6.2%   | 4.1.15   | A7211B4E35 |
| 1186:4200 | 1186:1103 | D-Link System   | DFE-520TX Fast Ethern... | 100%   |          | 790E740601 |
| 14e4:52a3 | d3a6:afcd | Broadcom Lim... | Ethernet controller      | 100%   |          | 191BA97155 |
| 8086:107c | 8086:1376 | Intel           | 82541PI Gigabit Ether... | 7.1%   | 2.6.32   | F801FAB1AD |
| 8086:15b8 | 1043:8672 | Intel           | Ethernet Connection (... | 2%     | 4.1.15   | 51B31F180E |

### Net/wireless (PCI)

29 out of 660 (4.39%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8400 | 1186:3b01 | Texas Instru... | ACX 100 22Mbps Wirele... | 100%   |          | 92B50659EB |
| 104c:9066 | 1086:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | DBFFE622A8 |
| 104c:9066 | 1186:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | A22609B54B |
| 10ec:8190 | 10ec:8190 | Realtek Semi... | RTL8190 802.11n PCI W... | 100%   |          | AF84B8FA95 |
| 10ec:8821 | 1a3b:2161 | Realtek Semi... | RTL8821AE 802.11ac PC... | 10.5%  | 3.14.44  | 5EEDC9CEE8 |
| 10ec:b723 | 1025:b734 | Realtek Semi... | RTL8723BE PCIe Wirele... | 2.9%   | 3.14.39  | 09F2C29527 |
| 10ec:b723 | 103c:2231 | Realtek Semi... | RTL8723BE PCIe Wirele... | 26.2%  | 3.14.15  | B301F51204 |
| 10ec:b723 | 10ec:b729 | Realtek Semi... | RTL8723BE PCIe Wirele... | 21.3%  | 3.14.44  | FD5BC52C49 |
| 10ec:b723 | 17aa:b728 | Realtek Semi... | RTL8723BE PCIe Wirele... | 20%    | 3.14.39  | 02D1977887 |
| 10ec:b723 | 17aa:b736 | Realtek Semi... | RTL8723BE PCIe Wirele... | 10.3%  | 3.14.53  | 8C16B6C71F |
| 10ec:b723 | 1a3b:2159 | Realtek Semi... | RTL8723BE PCIe Wirele... | 3.1%   | 3.14.44  | DDF48A7B95 |
| 10ec:b723 | 1b9a:2485 | Realtek Semi... | RTL8723BE PCIe Wirele... | 7.1%   | 4.1.19   | D57B5C86E0 |
| 11ab:1fa6 | 1043:138f | Marvell Tech... | Marvell W8300 802.11 ... | 100%   |          | 132128B023 |
| 11ab:1faa | 11ab:1faa | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | D686C53485 |
| 11ab:1faa | 1385:6b00 | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | 698A088620 |
| 14c3:7630 | 103c:197c | MEDIATEK        | MT7630e 802.11bgn Wir... | 27.8%  | 4.1.3    | A7E6CBC45B |
| 14c3:7630 | 105b:e074 | MEDIATEK        | MT7630e 802.11bgn Wir... | 47.8%  | 3.14.44  | 088B239273 |
| 14c3:7630 | 105b:e084 | MEDIATEK        | MT7630e 802.11bgn Wir... | 66.7%  | 4.9.41   | 82C19DDA3E |
| 168c:0042 | 11ad:0806 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 50%    | 4.4.0    | ECB6A89DFC |
| 168c:0042 | 11ad:08a6 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 5.6%   | 4.9.9    | E7395D0EE2 |
| 168c:0042 | 17aa:0901 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 6.2%   | 4.9.9    | C23D0EF968 |
| 168c:0042 | 17aa:4035 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 2.7%   | 4.8.0    | C3352134E9 |
| 1814:3062 | 1814:3062 | Ralink          | RT3062 Wireless 802.1... | 16.7%  | 3.14.44  | 9D9E2DB550 |
| 1814:5592 | 1043:851a | Ralink          | RT5592 PCIe Wireless ... | 100%   |          | 45CCD71213 |
| 8086:095a | 8086:5400 | Intel           | Wireless 7265            | 16.7%  | 4.1.25   | 0A99E4D896 |
| 8086:24f3 | 8086:1010 | Intel           | Wireless 8260            | 5%     | 4.1.15   | 43DF678BD3 |
| 8086:2526 | 8086:0014 | Intel           | Wireless-AC 9260         | 33.3%  | 4.16.13  | B078D35C2C |
| 8086:3165 | 8086:4010 | Intel           | Wireless 3165            | 1.6%   | 4.1.15   | 5738D326F6 |
| 8086:3166 | 8086:4210 | Intel           | Intel Dual Band Wirel... | 2.6%   | 4.1.15   | 18379EBD5C |

### Network (PCI)

6 out of 469 (1.28%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1006:3106 | 1086:1405 | Reply Group     | Reply Ethernet contro... | 100%   |          | F597A38FF5 |
| 10ec:b822 | 1043:8746 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 100%   |          | 27EB064D7D |
| 10ec:d723 | 103c:8319 | Realtek Semi... | Realtek Network contr... | 83.3%  | 4.9.87   | A0EB144818 |
| 12d0:2103 | 12d0:2103 | GDE Systems     | GDE Network controller   | 100%   |          | 8C5E6472B2 |
| 168c:004a | 15aa:4035 | Qualcomm Ath... | Network controller       | 100%   |          | 04F6BB6978 |
| 1810:3060 | 8001:0000 |                 | Network controller       | 100%   |          | CFD57C3B89 |

### Sound (PCI)

23 out of 5159 (0.45%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0045:c061 | 0045:c061 |                 | Audio device             | 100%   |          | 8D884B92FA |
| 1002:1314 | 1025:0520 | AMD/ATI         | Wrestler HDMI Audio      | 9.1%   | 3.14.44  | BF118AA31C |
| 1002:4383 | 1025:0520 | AMD/ATI         | SBx00 Azalia (Intel HDA) | 9.1%   | 3.14.44  | BF118AA31C |
| 1002:4383 | 1043:836c | AMD/ATI         | SBx00 Azalia (Intel HDA) | 0.5%   | 3.14.44  | B2C845B843 |
| 1002:9840 | 17aa:2219 | AMD/ATI         | Kabini HDMI/DP Audio     | 50%    | 4.9.60   | 94058A82CA |
| 1002:aab0 | 1043:aab0 | AMD/ATI         | Cape Verde/Pitcairn H... | 0.5%   | 3.14.22  | 71ABA86389 |
| 1022:780d | 1043:86c7 | AMD             | FCH Azalia Controller    | 50%    | 4.9.14   | 71ABA86389 |
| 10de:006b | 1043:0c11 | Nvidia          | nForce Audio Processi... | 100%   |          | 75D94681B0 |
| 10de:006b | 147b:1c00 | Nvidia          | nForce Audio Processi... | 100%   |          | CB892B4614 |
| 10de:03f0 | 1458:a002 | Nvidia          | MCP61 High Definition... | 0.7%   | 3.14.15  | 9D9E2DB550 |
| 10de:0bee |           | Nvidia          | GF116 High Definition... | 1.5%   | 3.14.39  | 77909796EC |
| 13f2:0111 |           | Ford Microel... |                          | 100%   |          | 95162A226D |
| 13f2:0111 | ffff:ffff | Ford Microel... | Multimedia audio cont... | 100%   |          | 95162A226D |
| 13f6:8788 | 1043:8463 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | 9E13784BB3 |
| 13f6:8788 | 1043:855e | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | EE53639037 |
| 8086:0c0c | 8086:0c0c | Intel           | Xeon E3-1200 v3/4th G... | 100%   |          | 77909796EC |
| 8086:0f28 | 17aa:3907 | Intel           | Atom Processor Z36xxx... | 100%   |          | 6D960BD235 |
| 8086:0f28 | 8086:0f28 | Intel           | Atom Processor Z36xxx... | 100%   |          | 185203390D |
| 8086:1c20 | 1043:8445 | Intel           | 6 Series/C200 Series ... | 0.5%   | 3.10.34  | 1678EE56C3 |
| 8086:1e20 | 1458:a002 | Intel           | 7 Series/C210 Series ... | 1%     | 3.10.42  | 740BF21A40 |
| 8086:22a8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | E6EE947879 |
| 8086:27d8 | 1462:104e | Intel           | NM10/ICH7 Family High... | 25%    | 4.1.15   | 5F15F028A8 |
| 8086:8c20 | 8086:8c20 | Intel           | 8 Series/C220 Series ... | 100%   |          | 77909796EC |

### Storage (PCI)

34 out of 146 (23.29%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1106:401a | 1071:9515 | VIA Technolo... | Storage controller       | 100%   |          | E028F277D4 |
| 1217:7130 | 1025:010d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | E24ADF3578 |
| 1217:7130 | 1025:011a | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 69380B60FC |
| 1217:7130 | 1025:0123 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B127BEAD10 |
| 1217:7130 | 1025:0124 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 1F2C670EC4 |
| 1217:7130 | 1025:012b | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 1190AECE7C |
| 1217:7130 | 1025:013c | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 879F60B1BF |
| 1217:7130 | 1028:026f | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 26F4ADE961 |
| 1217:7130 | 1028:0273 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 67689DAFA7 |
| 1217:7130 | 1071:8258 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 98006DB3BD |
| 1217:7130 | 107b:0696 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | E9F51C8451 |
| 1217:7130 | 10cf:13c6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 7B7919A092 |
| 1217:7130 | 10cf:143d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | D834A892F8 |
| 1217:7130 | 1179:ff50 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 5781A29611 |
| 1217:7130 | 1462:3fbb | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | FDCEAF9E02 |
| 1217:7130 | 1462:3fc1 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 278EF4A255 |
| 1217:7130 | 1462:3fe9 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 3F64CDD242 |
| 1217:7130 | 1462:3ff3 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 717F2BB4DB |
| 1217:7130 | 1462:4327 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 59A1BF0CA5 |
| 1217:7130 | 1462:63f6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | BA35BAD99E |
| 1217:7130 | 1631:0188 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 856B9A1A68 |
| 1217:7130 | 1734:10c7 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | A8295DF38F |
| 1217:8130 | 1025:019f | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 806ABC807D |
| 1217:8130 | 1028:02bc | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | B935B9FA3A |
| 1217:8130 | 10cf:1568 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | C2AA02F6B3 |
| 1217:8130 | 1179:ff50 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 3308602AF5 |
| 1217:8231 | 1028:0493 | O2 Micro        | Storage controller       | 100%   |          | 14051E2B63 |
| 1217:8330 | 1028:04a3 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | DBBEB2486E |
| 1217:8330 | 1028:04a4 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | A9FA71C0AE |
| 1217:8331 | 1028:0494 | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 9C03550D26 |
| 1217:8331 | 1028:049a | O2 Micro        | O2 Flash Memory Card     | 100%   |          | C77D4DC6A6 |
| 1217:8331 | 1028:049b | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 1EAB5F3026 |
| ace1:0005 | ace1:0005 |                 | Storage controller       | 100%   |          | 22F215C605 |
| ace1:0006 | ace1:0006 |                 | Storage controller       | 100%   |          | EF20304D33 |

### Storage/ata (PCI)

1 out of 2185 (0.05%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 11ab:6141 | 1043:81d6 | Marvell Tech... | 88SE614x SATA II PCI-... | 100%   |          | 12AE1A5665 |

### Storage/raid (PCI)

3 out of 190 (1.58%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1022:43bd | 1b21:1062 | AMD             | RAID bus controller      | 100%   |          | 94B0CBF647 |
| 1095:1114 | 1095:5114 | Silicon Image   | RAID bus controller      | 100%   |          | 126A2B0E4F |
| 1590:0045 | 1590:0045 | Hewlett-Packard | RAID bus controller      | 100%   |          | 3FAC52AF81 |

### System peripheral (PCI)

81 out of 475 (17.05%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 103c:3306 | 103c:3381 | Hewlett-Packard | Integrated Lights-Out... | 20%    | 2.6.32   | 2D74AD691D |
| 104c:8201 | 103c:08b0 | Texas Instru... | PCI1620 Firmware Load... | 100%   |          | 316E375A5C |
| 104c:8204 | 1028:014e | Texas Instru... | PCI7410/7510/7610 PCI... | 100%   |          | 0493B906A1 |
| 1179:0805 | 1179:0001 | Toshiba Amer... | SD TypA Controller       | 80%    | 4.1.34   | 6ED70A9B46 |
| 1180:0576 | 10cf:1256 | Ricoh           | R5C576 SD Bus Host Ad... | 100%   |          | 4DCFB332DF |
| 1180:0852 | 1043:1877 | Ricoh           | xD-Picture Card Contr... | 4.1%   | 3.0.28   | 70CC866946 |
| 1180:e230 | 1028:02bd | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 31D62139B3 |
| 1180:e230 | 1028:02fe | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 4DA3A91131 |
| 1180:e230 | 1028:0401 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 6006F3386E |
| 1180:e230 | 1028:0402 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | A84F1BF78D |
| 1180:e230 | 1028:0413 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 16783EA6FB |
| 1180:e230 | 103c:1455 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | E4E639B7D7 |
| 1180:e230 | 103c:146d | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 624F76AEDC |
| 1180:e230 | 103c:1471 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 81B7639BA6 |
| 1180:e230 | 103c:1722 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 2D885D19FD |
| 1180:e230 | 103c:1726 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 759D141031 |
| 1180:e230 | 104d:905a | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 94BF85CB32 |
| 1180:e230 | 104d:9060 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | F3D7A20E22 |
| 1180:e230 | 104d:9066 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | A11EA53B6C |
| 1180:e230 | 104d:9069 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | C8B9D21B89 |
| 1180:e230 | 104d:9071 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | F48EC5BD0F |
| 1180:e230 | 104d:9072 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | DA9CBAC74B |
| 1180:e230 | 1179:0001 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | E77127AAC2 |
| 1180:e230 | 1179:ff40 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | C8BC53F831 |
| 1180:e230 | 17aa:2134 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | B08518378D |
| 1180:e232 | 104d:907e | Ricoh           | System peripheral        | 100%   |          | BFBC69664C |
| 1180:e232 | 104d:9081 | Ricoh           | System peripheral        | 100%   |          | AEC874178B |
| 1180:e232 | 104d:9083 | Ricoh           | System peripheral        | 100%   |          | 71851F6A64 |
| 1180:e232 | 104d:9086 | Ricoh           | System peripheral        | 100%   |          | EB8193522C |
| 1180:e232 | 104d:9089 | Ricoh           | System peripheral        | 100%   |          | 0E64E747B5 |
| 1180:e232 | 104d:908e | Ricoh           | System peripheral        | 100%   |          | FC55716771 |
| 1180:e232 | 104d:9095 | Ricoh           | System peripheral        | 100%   |          | FBA8485786 |
| 1180:e232 | 104d:9097 | Ricoh           | System peripheral        | 100%   |          | 7685534B8E |
| 1180:e232 | 1179:0001 | Ricoh           | System peripheral        | 100%   |          | 8F76C37692 |
| 14e4:16be | 1025:0504 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | EB4279887A |
| 14e4:16be | 1025:0599 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 3689EE7B19 |
| 14e4:16be | 1025:0605 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 4ABA261C6D |
| 14e4:16be | 1025:0647 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | D950940586 |
| 14e4:16bf | 1025:0504 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | EB4279887A |
| 14e4:16bf | 1025:0599 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 3689EE7B19 |
| 14e4:16bf | 1025:0605 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 4ABA261C6D |
| 14e4:16bf | 1025:0647 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | D950940586 |
| 197b:2384 | 1019:2238 | JMicron Tech... | xD Host Controller       | 100%   |          | 7E782321C8 |
| 197b:2384 | 1025:013b | JMicron Tech... | xD Host Controller       | 100%   |          | 3C347BEC2E |
| 197b:2384 | 1025:013e | JMicron Tech... | xD Host Controller       | 100%   |          | B563FF6430 |
| 197b:2384 | 1025:0142 | JMicron Tech... | xD Host Controller       | 100%   |          | E10FB8CE91 |
| 197b:2384 | 1025:0143 | JMicron Tech... | xD Host Controller       | 100%   |          | 310A169187 |
| 197b:2384 | 1025:0145 | JMicron Tech... | xD Host Controller       | 100%   |          | BAB0D5B451 |
| 197b:2384 | 1025:0146 | JMicron Tech... | xD Host Controller       | 100%   |          | 2D9126A5BF |
| 197b:2384 | 1025:015b | JMicron Tech... | xD Host Controller       | 100%   |          | D9272C7894 |
| 197b:2384 | 1025:0160 | JMicron Tech... | xD Host Controller       | 100%   |          | BBCDDB4D27 |
| 197b:2384 | 1025:0200 | JMicron Tech... | xD Host Controller       | 100%   |          | 13537074DF |
| 197b:2384 | 1025:042f | JMicron Tech... | xD Host Controller       | 100%   |          | 1395FA2E0F |
| 197b:2384 | 103c:2aa2 | JMicron Tech... | xD Host Controller       | 100%   |          | D8AA06CBF6 |
| 197b:2384 | 103c:2aa6 | JMicron Tech... | xD Host Controller       | 100%   |          | 9D61E4EA0B |
| 197b:2384 | 103c:30f4 | JMicron Tech... | xD Host Controller       | 100%   |          | 5FBA4BFB17 |
| 197b:2384 | 103c:30f7 | JMicron Tech... | xD Host Controller       | 100%   |          | 0922CD3C27 |
| 197b:2384 | 103c:30fb | JMicron Tech... | xD Host Controller       | 100%   |          | 762D293955 |
| 197b:2384 | 103c:3600 | JMicron Tech... | xD Host Controller       | 100%   |          | 560896EB09 |
| 197b:2384 | 103c:3603 | JMicron Tech... | xD Host Controller       | 100%   |          | 3191678465 |
| 197b:2384 | 103c:3624 | JMicron Tech... | xD Host Controller       | 100%   |          | 5B28FAF10B |
| 197b:2384 | 103c:3628 | JMicron Tech... | xD Host Controller       | 100%   |          | 3E6DDADA1D |
| 197b:2384 | 103c:363e | JMicron Tech... | xD Host Controller       | 100%   |          | 95860AB870 |
| 197b:2384 | 103c:3659 | JMicron Tech... | xD Host Controller       | 100%   |          | 99DDBBF195 |
| 197b:2384 | 103c:7001 | JMicron Tech... | xD Host Controller       | 100%   |          | CD1057E220 |
| 197b:2384 | 103c:7010 | JMicron Tech... | xD Host Controller       | 100%   |          | 6E70B36184 |
| 197b:2384 | 1043:1a07 | JMicron Tech... | xD Host Controller       | 100%   |          | 8BDF051BC4 |
| 197b:2384 | 1179:fd30 | JMicron Tech... | xD Host Controller       | 100%   |          | 891CD49EC9 |
| 197b:2384 | 1179:ff02 | JMicron Tech... | xD Host Controller       | 100%   |          | 17C890C4D4 |
| 197b:2384 | 1179:ff08 | JMicron Tech... | xD Host Controller       | 100%   |          | F2679655D8 |
| 197b:2384 | 152d:0834 | JMicron Tech... | xD Host Controller       | 100%   |          | C6D0242C42 |
| 197b:2384 | 1558:0806 | JMicron Tech... | xD Host Controller       | 100%   |          | F3BF4D62C0 |
| 197b:2384 | 1734:113d | JMicron Tech... | xD Host Controller       | 100%   |          | BD5D293529 |
| 197b:2384 | 17aa:2130 | JMicron Tech... | xD Host Controller       | 100%   |          | 50CA916983 |
| 197b:2384 | 17aa:3602 | JMicron Tech... | xD Host Controller       | 100%   |          | 60AE7E3358 |
| 197b:2384 | 17aa:3881 | JMicron Tech... | xD Host Controller       | 100%   |          | 7F669E0390 |
| 197b:2387 | 17aa:3921 | JMicron Tech... | SD/MMC Host Controller   | 100%   |          | 57733D4AEE |
| 197b:2389 | 17aa:3924 | JMicron Tech... | xD Host Controller       | 100%   |          | 57733D4AEE |
| 197b:2394 | 1462:107f | JMicron Tech... | xD Host Controller       | 100%   |          | 4D22D14A1D |
| 197b:2394 | 17aa:3976 | JMicron Tech... | xD Host Controller       | 100%   |          | 502AFED52F |
| 197b:2394 | 17aa:3977 | JMicron Tech... | xD Host Controller       | 100%   |          | F50039D1B3 |

### Tv card (PCI)

2 out of 168 (1.19%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 11de:6057 | 1031:7efe | Zoran           | ZR36057PQC Video cutt... | 50%    | 3.14.44  | BEB1083A7F |
| 11de:6057 | 1031:d801 | Zoran           | ZR36057PQC Video cutt... | 100%   |          | F700FF20C6 |

### Usb controller (PCI)

2 out of 9735 (0.02%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1106:3483 | 1458:5007 | VIA Technolo... | VL805 USB 3.0 Host Co... | 0.7%   | 3.14.44  | 96703A2AD7 |
| 8086:22b7 | 8086:7270 | Intel           | USB Controller           | 6.2%   | 4.9.9    | 0533FA1449 |

USB Devices
-----------

Non-100% value in the 'Missed' column indicates that the driver for a device is available
in the latest kernel versions. You can find corresponding hwinfo reports for listed devices
by a probe ID.

Missed — percentage of probes with missed driver for the device,
Linux  — the minimum Linux kernel version in which the driver was found,
Probe  — latest probe ID with missed driver for the device.

### Audio (USB)

4 out of 28 (14.29%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:0a0b | Logitech        | ClearChat Pro USB        | 100%   |          | 56D5984A14 |
| 0644:8030 | TEAC            | US-1800                  | 100%   |          | 5D4A91211F |
| 0955:7002 | Nvidia          | stereo controller        | 100%   |          | FC2416C79A |
| 1235:8016 | Focusrite-No... | Focusrite Scarlett 2i2   | 50%    | 4.9.20   | F16ADBF7F3 |

### Bluetooth (USB)

11 out of 259 (4.25%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0489:e069 | Foxconn / Ho... | BT                       | 95.8%  | 4.9.41   | 088B239273 |
| 04ca:2006 | Lite-On Tech... | BCM43142A0 Bluetooth ... | 14%    | 4.0.8    | 805C7CD772 |
| 04ca:2007 | Lite-On Tech... | Broadcom BCM43142A0 B... | 14.6%  | 4.1.7    | BAA62D56E7 |
| 04ca:2009 | Lite-On Tech... | BCM43142A0               | 22.2%  | 4.0.2    | 14539CFCC1 |
| 05e1:0100 | Syntek          | 802.11g + Bluetooth W... | 100%   |          | FB86FAD6D2 |
| 0cf3:3004 | Qualcomm Ath... | AR3012 Bluetooth 4.0     | 0.5%   | 3.10.51  | 1DD6BF2D41 |
| 0cf3:3008 | Qualcomm Ath... | Bluetooth (AR3011)       | 2.3%   | 3.14.25  | F430167968 |
| 0e8d:763e | MediaTek        | MT7630e Bluetooth Ada... | 100%   |          | A7E6CBC45B |
| 105b:e065 | Foxconn Inte... | BCM43142A0 Bluetooth ... | 21.2%  | 4.0.1    | F39685A972 |
| 13d3:3392 | IMC Networks    | Azurewave 43228+20702... | 100%   |          | 337156D639 |
| 413c:8143 | Dell            | BCM20702A0               | 100%   |          | AE4C0F8B6B |

### Camera (USB)

23 out of 1269 (1.81%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 041e:400d | Creative Tec... | Webcam PD1001            | 100%   |          | 1892C5C88C |
| 041e:4039 | Creative Tec... | Webcam Live! Effects     | 100%   |          | EB3A6BB1E4 |
| 0458:702a | KYE Systems ... | WebCAM USB2.0            | 100%   |          | 3D86369A82 |
| 04f2:b270 | Chicony Elec... | HP HD Webcam [Fixed]     | 16.7%  | 3.14.44  | C6E683B39B |
| 04f2:b3b2 | Chicony Elec... | TOSHIBA Web Camera - FHD | 100%   |          | 550460AAAC |
| 04f2:b5f7 | Chicony Elec... | HD WebCam                | 33.3%  | 4.9.20   | 51AC6D49F9 |
| 0547:6512 | Anchor Chips    | UCMOS05100KPA Microsc... | 100%   |          | C824174CB6 |
| 05ca:1830 | Ricoh           | Visual Communication ... | 100%   |          | 4C62F660CE |
| 05ca:1870 | Ricoh           | Webcam 1000              | 100%   |          | 94E998BCAF |
| 093a:7011 | Pixart Imaging  | Digital Wireless Camera  | 100%   |          | 0D741D736E |
| 0ac8:3450 | Z-Star Micro... | Vimicro USB Camera (A... | 0.5%   | 3.14.22  | 3C44204AA0 |
| 0ac8:c326 | Z-Star Micro... | Namuga 1.3M Webcam       | 11.1%  | 4.1.15   | 3AD0FF0E13 |
| 0ac8:c40a | Z-Star Micro... | A4 TECH USB2.0 PC Cam... | 0.4%   | 3.10.34  | B2C845B843 |
| 0b97:8381 | O2 Micro        | Mini S USB2.0 Camera     | 100%   |          | 74DE04A0B0 |
| 0bda:58be | Realtek Semi... | Laptop_Integrated_Web... | 25%    | 4.1.15   | A7211B4E35 |
| 0c45:6350 | Microdia        | USB 2.0 Camera           | 100%   |          | 34DDCDDC0E |
| 0e8d:200b | MediaTek        | Power                    | 100%   |          | F2CD8A3FFB |
| 174f:5a35 | Syntek          | Sonix 1.3MPixel USB 2... | 2.1%   | 3.14.33  | 0A87DE5887 |
| 174f:6a33 | Syntek          | Web Cam - Asus F3SA, ... | 100%   |          | 932CA241F8 |
| 174f:6a51 | Syntek          | 2.0MPixel Web Cam - A... | 100%   |          | 39E3030E0A |
| 1782:4011 | Spreadtrum C... | Android                  | 100%   |          | 9869646781 |
| 18ec:3399 | Arkmicro Tec... | USB2.0 PC CAMERA         | 1.1%   | 3.14.25  | 9D9E2DB550 |
| 1b17:6111 | DarkHorse .     | USB2.0 Web Camera        | 100%   |          | 6E9BA31D2B |

### Card reader (USB)

4 out of 8 (50%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0b0c:003f | Todos AB        | Todos C400 smartcard ... | 100%   |          | 251D958CA9 |
| 0bda:0139 | Realtek Semi... | RTS5139 Card Reader C... | 0.3%   | 3.10.34  | EF015B9C0F |
| 0bda:0150 | Realtek Semi... | USB 2.0 Card Reader      | 100%   |          | 3C44204AA0 |
| 0d8c:5200 | C-Media Elec... | Mass Storage Controll... | 100%   |          | 15ED4815BD |

### Chipcard (USB)

26 out of 27 (96.30%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0403:e3b4 | Future Techn... | Parsec Desktop Reader... | 100%   |          | 775160993D |
| 0529:0620 | Aladdin Know... | Token JC                 | 91.7%  | 3.14.25  | 39F3C43A6B |
| 058f:9520 | Alcor Micro     | EMV Certified Smart C... | 100%   |          | 6BB6CFD197 |
| 058f:9540 | Alcor Micro     | AU9540 Smartcard Reader  | 96.2%  | 4.13.0   | 723C7E964F |
| 072f:90cc | Advanced Car... | ACR38 SmartCard Reader   | 100%   |          | 55834A1077 |
| 072f:90de | Advanced Car... | Token USB 64K            | 33.3%  | 4.1.25   | A8A89AC09A |
| 072f:b000 | Advanced Car... | ACR3901U                 | 100%   |          | A44B651190 |
| 076b:1021 | OmniKey         | CardMan 1021             | 100%   |          | 24366329C2 |
| 076b:4321 | OmniKey         | CardMan 4321             | 100%   |          | 3191678465 |
| 08e6:3438 | Gemalto (was... | GemPC Key SmartCard R... | 100%   |          | 6BDD8BE020 |
| 08e6:34ec | Gemalto (was... | Compact Smart Card Re... | 100%   |          | 0A15E23212 |
| 0a5c:5800 | Broadcom        | BCM5880 Secure Applic... | 98.8%  | 3.10.36  | 14051E2B63 |
| 0a5c:5801 | Broadcom        | BCM5880 Secure Applic... | 98.9%  | 3.16.7   | EAA58F3A1F |
| 0a5c:5804 | Broadcom        | BCM5880 Secure Applic... | 100%   |          | 19E75EF49D |
| 0a5c:5832 | Broadcom        | 5880                     | 100%   |          | 364F29C9B1 |
| 0a89:0025 | Aktiv           | Rutoken lite             | 50%    | 4.1.25   | 8FA80B8A39 |
| 0b97:7762 | O2 Micro        | Oz776 SmartCard Reader   | 100%   |          | 293BAD8F02 |
| 0b97:7772 | O2 Micro        | OZ776 CCID Smartcard ... | 97.5%  | 4.16.9   | 98BDAAC89B |
| 0bda:0165 | Realtek Semi... | Smart Card Reader Int... | 100%   |          | 9664AA0934 |
| 0c4b:9102 | Reiner SCT K... | cyberJack RFID basis ... | 100%   |          | D772023A07 |
| 0ca6:00a0 | Castles Tech... | EZCCID Smart Card Reader | 100%   |          | 3DC7A36CB3 |
| 0dc3:1004 | Athena Smart... | ASEDrive CCID            | 100%   |          | FB13C4ACE3 |
| 147e:2020 | Upek            | TouchChip Fingerprint... | 100%   |          | 1FD195EA79 |
| 17ef:1003 | Lenovo          | Integrated Smart Card... | 100%   |          | 0476F6CAB9 |
| 23a0:0004 | BIFIT           | iBank2Key                | 100%   |          | A8A89AC09A |
| 24dc:0101 | ARDS            | JaCarta                  | 100%   |          | DA308A78C4 |

### Converter (USB)

2 out of 3 (66.67%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0403:1237 | Future Techn... | Z397 GUARD Converter     | 100%   |          | 00A5CE299A |
| 110a:1110 | Moxa Technol... | UPort 1110 1-port RS-... | 100%   |          | 3864E6C70F |

### Disk (USB)

6 out of 922 (0.65%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 048d:1336 | Integrated T... | SD/MMC Cardreader        | 0.4%   | 3.14.22  | 7E7FB78F58 |
| 058f:6362 | Alcor Micro     | Flash Card Reader/Writer | 0.2%   | 3.8.12   | 0D4B7AD71C |
| 05e3:0723 | Genesys Logic   | GL827L SD/MMC/MS Flas... | 4%     | 3.14.33  | 5295F40FC3 |
| 1005:b113 | Apacer Techn... | Handy Steno/AH123 / H... | 0.5%   | 3.0.28   | 8652B8318D |
| 13fd:1617 | Initio          | Flash Padlock            | 100%   |          | 95CE4B3495 |
| 5136:4678 | Generic         | Flash Disk 2.0 8.3886... | 40%    | 4.1.38   | C1841B0A29 |

### Dvb card (USB)

3 out of 17 (17.65%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 07ca:0830 | AVerMedia Te... | H830 USB Hybrid DVB-T    | 100%   |          | 5F72AF687D |
| 0bda:2838 | Realtek Semi... | RTL2838 DVB-T            | 16.7%  | 3.14.25  | F3FC00F966 |
| eb1a:5013 | eMPIA Techno... | USB 2883 Device          | 100%   |          | 5DD14F9164 |

### Fingerprint reader (USB)

32 out of 33 (96.97%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0483:2016 | STMicroelect... | Fingerprint Reader       | 100%   |          | F9B5D49091 |
| 05ba:0002 | DigitalPersona  | Fingerprint Scanner, ... | 100%   |          | AE361E5F23 |
| 08ff:1600 | AuthenTec       | AES1600                  | 100%   |          | D8B4DE039A |
| 08ff:168b | AuthenTec       | Fingerprint Sensor       | 100%   |          | E77127AAC2 |
| 08ff:168f | AuthenTec       | AES1660 Fingerprint S... | 100%   |          | 2192F26242 |
| 08ff:2500 | AuthenTec       | AES2501                  | 100%   |          | 4DCFB332DF |
| 08ff:2550 | AuthenTec       | AES2550 Fingerprint S... | 100%   |          | 9218F197A1 |
| 08ff:2580 | AuthenTec       | AES2501 Fingerprint S... | 100%   |          | E5C0601D04 |
| 08ff:2665 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 859C14C1FB |
| 08ff:2683 | AuthenTec       | Fingerprint Sensor       | 100%   |          | FF16BAA7D4 |
| 08ff:2691 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 79E75DF44E |
| 08ff:2810 | AuthenTec       | AES2810                  | 100%   |          | 0DB5880016 |
| 138a:0001 | Validity Sen... | VFS101 Fingerprint Re... | 100%   |          | 8CB1C6C855 |
| 138a:0005 | Validity Sen... | VFS301 Fingerprint Re... | 100%   |          | C11A7BCF0D |
| 138a:0007 | Validity Sen... | VFS451 Fingerprint Re... | 100%   |          | 759D141031 |
| 138a:0008 | Validity Sen... | VFS300 Fingerprint Re... | 100%   |          | D3246E9947 |
| 138a:0010 | Validity Sen... | VFS Fingerprint sensor   | 100%   |          | E6F26F46C2 |
| 138a:0011 | Validity Sen... | VFS5011 Fingerprint R... | 100%   |          | FDA3476D59 |
| 138a:0017 | Validity Sen... | VFS 5011 fingerprint ... | 100%   |          | CF2F96CF72 |
| 138a:0018 | Validity Sen... | Fingerprint scanner      | 100%   |          | 81AE69BF52 |
| 138a:003c | Validity Sen... | VFS471 Fingerprint Re... | 100%   |          | AD80B34D19 |
| 138a:003d | Validity Sen... | VFS491                   | 100%   |          | 43578C0823 |
| 138a:003f | Validity Sen... | VFS495 Fingerprint Re... | 100%   |          | 6B58CB62F6 |
| 138a:0050 | Validity Sen... | Swipe Fingerprint Sensor | 100%   |          | 859218E7D2 |
| 138a:0090 | Validity Sen... | VFS7500 Touch Fingerp... | 100%   |          | 6FA0843228 |
| 138a:0091 | Validity Sen... | VFS7552 Touch Fingerp... | 100%   |          | 8E3B752DEE |
| 147e:1000 | Upek            | Biometric Touchchip/T... | 100%   |          | CB763F4F13 |
| 147e:1001 | Upek            | TCS5B Fingerprint sensor | 100%   |          | C8B9D21B89 |
| 147e:1002 | Upek            | Biometric Touchchip/T... | 100%   |          | A211D2122B |
| 147e:2016 | Upek            | Biometric Touchchip/T... | 100%   |          | E8FE24FA20 |
| 1c7a:0603 | LighTuning T... | EgisTec ES603            | 100%   |          | B0EBF85C1D |
| 1c7a:0801 | LighTuning T... | Fingerprint Reader       | 100%   |          | 8165335824 |

### Hardware key (USB)

4 out of 4 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0471:485d | Philips (or ... | Senselock SenseIV v2.x   | 100%   |          | E4A6E39276 |
| 0a89:0003 | Aktiv           | Guardant Stealth/Net II  | 100%   |          | C6EC8326CA |
| 0a89:0020 | Aktiv           | Rutoken S                | 75%    | 3.14.15  | 39F3C43A6B |
| 14a8:0001 | Soft protect... | Soft protection devic... | 100%   |          | 568CDC2D31 |

### Hasp (USB)

1 out of 1 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0529:0001 | Aladdin Know... | HASP copy protection ... | 100%   |          | 35AA872865 |

### Hub (USB)

1 out of 185 (0.54%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0451:1446 | Texas Instru... | TUSB2040/2070 Hub        | 100%   |          | 593A72A02B |

### Human interface (USB)

2 out of 198 (1.01%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 11ff:3341 |                 | USB Joystick             | 25%    | 4.1.7    | CD7FA9B160 |
| 1770:ff00 | MSI EPF USB     | MSI EPF USB / LED con... | 1.9%   | 3.14.39  | 1C47BC90E4 |

### Imaging (USB)

1 out of 2 (50%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04a7:04d0 | Visioneer       | Xerox DocuMate 5460      | 100%   |          | 4ABAC242CC |

### Input/keyboard (USB)

2 out of 818 (0.24%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0a5c:4502 | Broadcom        | Keyboard (Boot Interf... | 1.1%   | 3.0.28   | 0C3E26BCE7 |
| 0b05:17fd | ASUSTek Comp... | ASUS ROG Macrokey        | 33.3%  | 3.14.44  | C5777BA928 |

### Input/mouse (USB)

6 out of 744 (0.81%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0458:003a | KYE Systems ... | NetScroll+ Mini Trave... | 0.2%   | 3.10.34  | 5599435B69 |
| 045e:0040 | Microsoft       | Wheel Mouse Optical      | 2%     | 3.14.25  | BFCD766C51 |
| 046d:c06c | Logitech        | Optical Mouse            | 0.5%   | 2.6.32   | C6690BB6D9 |
| 04b4:0033 | Cypress Semi... | Mouse                    | 1.2%   | 3.14.25  | 4BCDE0B215 |
| 413c:8158 | Dell            | Integrated Touchpad /... | 80%    | 3.14.44  | 27413A0BD2 |
| 413c:8162 | Dell            | Integrated Touchpad [... | 76.5%  | 3.14.33  | 3D94981F5F |

### Modem (USB)

2 out of 62 (3.23%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04e8:6773 | Samsung Elec... | HSPA Modem               | 100%   |          | 3AD0FF0E13 |
| 0baf:00ec | U.S. Robotics   | 56K Faxmodem             | 100%   |          | DB286E3DD1 |

### Net/wimax (USB)

3 out of 5 (60%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 8086:0186 | Intel           | WiMAX Connection 2400m   | 4.8%   | 3.14.44  | A7211B4E35 |
| 8086:1406 | Intel           | WiMAX Connection 2400m   | 4.5%   | 3.10.19  | 5971AC1B90 |
| 8087:07d6 | Intel           | Centrino WiMAX 6150      | 13%    | 3.10.34  | D1BD6FB889 |

### Net/wireless (USB)

28 out of 127 (22.05%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0411:0242 | BUFFALO         | 802.11ac WLAN Adapter    | 100%   |          | 1A6E39D574 |
| 0457:0162 | Silicon Inte... | SiS162 usb Wireless L... | 100%   |          | D625F7E867 |
| 0846:9011 | NetGear         | WNDA3100v2 802.11abgn... | 100%   |          | 3B8C072C99 |
| 0846:9020 | NetGear         | WNA3100(v1) Wireless-... | 100%   |          | FFCF433D14 |
| 0b05:17d1 | ASUSTek Comp... | AC51 802.11a/b/g/n/ac... | 100%   |          | 3CBF6D38BA |
| 0b05:17db | ASUSTek Comp... | USB-AC50 802.11a/b/g/... | 100%   |          | 93C92CF446 |
| 0b05:1817 | ASUSTek Comp... | USB-AC68 802.11a/b/g/... | 100%   |          | 9639F147B5 |
| 0bda:0811 | Realtek Semi... | 802.11ac WLAN Adapter    | 100%   |          | AB74FDC0F5 |
| 0bda:8179 | Realtek Semi... | RTL8188EUS 802.11n Wi... | 0.5%   | 3.14.25  | 1678EE56C3 |
| 0bda:818b | Realtek Semi... | ACT-WNP-UA-005 802.11... | 55.6%  | 4.9.9    | 52A6238F08 |
| 0bda:8812 | Realtek Semi... | RTL8812AU 802.11a/b/g... | 25%    | 4.1.38   | 40AF662959 |
| 0bda:a811 | Realtek Semi... | RTL8811AU 802.11a/b/g... | 100%   |          | C0F433D67B |
| 0cde:0015 | Z-Com           | XG-705A 802.11g Wirel... | 100%   |          | B4E374835E |
| 0cf3:9271 | Qualcomm Ath... | AR9271 802.11n           | 0.5%   | 3.14.25  | E6A7D05EF4 |
| 13b1:003a | Linksys         | AE2500 802.11abgn Wir... | 100%   |          | 802B06DA23 |
| 13b1:003e | Linksys         | AE6000 802.11a/b/g/n/... | 100%   |          | 6F68EDE0BD |
| 13b1:003f | Linksys         | WUSB6300 802.11a/b/g/... | 80%    | 4.1.19   | A0B41E7AB4 |
| 13b1:0042 | Linksys         | WUSB6100M 802.11a/b/g... | 100%   |          | 5155142A94 |
| 148f:7601 | Ralink Techn... | MT7601U Wireless Adapter | 30.7%  | 3.14.33  | B0340A413E |
| 148f:760b | Ralink Techn... | MT7601U Wireless Adapter | 37.5%  | 3.14.33  | 335F9F48EE |
| 148f:761a | Ralink Techn... | MT7610U ("Archer T2U"... | 100%   |          | C0ED6FD808 |
| 2001:3314 | D-Link          | 802.11n WLAN Adapter     | 100%   |          | 1EE95C9EF0 |
| 2001:3315 | D-Link          | Wireless Adapter         | 50%    | 3.14.39  | D630B05372 |
| 2001:3319 | D-Link          | Wireless N Nano USB A... | 83.3%  | 4.1.38   | C5C35CEA92 |
| 2357:0101 | Realtek         | 802.11n NIC              | 50%    | 4.1.25   | 39787584D1 |
| 2357:0103 | Realtek         | Archer T4UH wireless ... | 50%    | 3.14.44  | D804242BA9 |
| 2357:0109 | Realtek         | 802.11n WLAN Adapter     | 36.4%  | 4.9.9    | 8DE11EB42D |
| 2357:010c | Realtek         | TL-WN722N v2             | 50%    | 4.9.41   | 27F51AD07D |

### Network (USB)

3 out of 141 (2.13%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0bda:b720 | Realtek Semi... | 802.11n WLAN Adapter     | 20%    | 4.4.1    | 6135515DEB |
| 2001:330f | D-Link          | DWA-125 11n Adapter      | 4.3%   | 3.14.44  | 01D21EA756 |
| 7392:a812 | Edimax Techn... | Edimax AC600 USB         | 28.6%  | 3.14.25  | FA09AEC26E |

### Tv card (USB)

1 out of 74 (1.35%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 07ca:0889 | AVerMedia Te... | AVerTV Satellite 2       | 100%   |          | 174EC665C6 |

### Video (USB)

5 out of 6 (83.33%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0fd9:0051 | Elgato Systems  | GameCapture HD           | 100%   |          | 05F988930D |
| 1164:1ee9 | YUAN High-Te... | Polaris AV Capture       | 100%   |          | 741E3E3C76 |
| 1b80:a41c | Afatech         | Polaris AV Capture       | 100%   |          | F20674C0B8 |
| 2304:0224 | Pinnacle Sys... | MovieBox Plus (710-USB)  | 100%   |          | 5F24B5D0A3 |
| 5555:3382 | Epiphan Systems | VGA2USB Frame Grabber    | 100%   |          | 37A831391B |

### Wireless (USB)

1 out of 11 (9.09%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 15a9:003a | Gemtek          | Modem YOTA 4G LTE        | 100%   |          | 02E0DBC8D3 |

