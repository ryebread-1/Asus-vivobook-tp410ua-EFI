<h1 align="center">Hackintosh the Asus Vivobook flip 14</h1>

<p align="center">
    <a href="https://www.apple.com/">
        <img src="https://img.shields.io/badge/Catalina-10.15.7-blue.svg"/></a>
    <a href="https://www.apple.com/macos/big-sur/">
        <img src="https://img.shields.io/badge/Big_Sur-11.6.5-blue.svg"></a>
    <a href="https://www.apple.com/macos/monterey/">
        <img src="https://img.shields.io/badge/Monterey-12.3.1-blue"></a>
    <a href="https://github.com/acidanthera/OpenCorePkg">
        <img src="https://img.shields.io/badge/OpenCore-0.8.3-blue"/></a>
</p>

#### I am not responsible for any damages you may cause.

#### If my work here helped you. Please write to me! It will make me very happy.

- Complete EFI is available in the releases page.
- I will try my best to keep the repo updated with the latest kexts and OpenCore version.
- This EFI is configured with Catalina, Big Sur, Monterey and Ventura.
- With every EFI update you retrieve from here please remember to go through the post install guide.  

## Update

### Recent |

<details>
<summary><strong> SUMMARY </strong></summary>
<br>

> ### Non-Fuctional

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| Fingerprint Reader                   | ❌   | `DISABLED` in BIOS to save power. |

> ### Video and Audio

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| Full Graphics Accleration (QE/CI)    | ✅   | `WhateverGreen.kext`  |
| Audio                      | ✅   | `AppleALC.kext` with Layout ID = 11|


> ### Power, Charge, Sleep and Hibernation

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| Battery Percentage Indication        | ✅   | `ECEnabler.kext`            | 
| iGPU Power Management                | ✅   | `XCPM`, enabled by `SSDT-PLUG.aml` |
| Battery Life                         | ✅   |  Similiar to Windows/Linux. |

> ### Input/ Output

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| WiFi                                 | ✅   | `native`  |
| Bluetooth                            | ✅   | `native`  |
|USB Ports                             | ✅   | `SSDT-EC-USBX-LAPTOP.aml`    |
|SD card reader                           | ✅   | `RealtekCardReader.kext`|

> ### Display, TrackPad, TrackPoint, and Keyboard

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| Brightness Adjustments | ✅  | `WhateverGreen.kext`, `SSDT-PNLF.aml`|
| TrackPad               | ✅  | `VoodooPS2Controller.kext` |
| Built-in Keyboard      | ✅  | `VoodooPS2Controller.kext` |

> ### macOS Continuity

| Feature                              | Status | Dependency          |
| :----------------------------------- | ------ | ------------------- |
| iCloud, iMessage, FaceTime           | ✅   | Whitelisted Apple ID, Valid SMBIOS  |
| AirDrop                              | ✅   | Working  |
| Time Machine                         | ✅   | Native  |

</details>

<details>
<summary><strong> REFERENCES </strong></summary>
<br>

Read these before you start:

- [dortania's Hackintosh guides](https://github.com/dortania).
- [dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/).
- [dortania's OpenCore Post Install Guide](https://dortania.github.io/OpenCore-Post-Install/).
- [dortania/ Getting Started with ACPI](https://dortania.github.io/Getting-Started-With-ACPI/).
- [dortania/ opencore multiboot](https://github.com/dortania/OpenCore-Multiboot).

</details>

<details>
<summary><strong> REQUIREMENTS </strong></summary>
<br>

- A macOS machine(optional): to create the macOS installer.
- Flash drive, 32GB or more for monterey and above, and 16gb for Big Sur and below.  
- [ProperTree](https://github.com/corpnewt/ProperTree) if you need to edit plist files on Windows.  
- [MaciASL](https://github.com/acidanthera/MaciASL), for patching ACPI tables and editing ACPI patches.
- [MountEFI](https://github.com/corpnewt/MountEFI) to quickly mount EFI partitions.  
- [IORegistryExplorer](https://developer.apple.com/downloads) 
- Patience and time, especially if this is your first time "hackintoshing".

</details>

<details>
<summary><strong> HARDWARE </strong></summary>
<br>

| Category  | Vivobook flip 14         |
| --------- | ------------------------ |
| CPU       | Intel Core i5-7200U      |
| SSD       | Samsung 870 Evo 250GB    |
| Display   | 14" screen hd 1920x1080p |
| WiFi card | Broadcom 4360ng.        |


</details>

<details>
<summary><strong> GETTING STARTED </strong></summary>
<br>

- Creating a macOS installer: refer to [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)

</details>

<details>
<summary><strong> BENCHMARKS </strong></summary>
</br>

- macOS 13.0, EFI OpenCore 0.8.3

| CPU            | Single-Core | Multi-Core |
| :------------- | ----------: | ---------: |
| Geekbench |            725      |       1790 |

| GPU            | OpenCL      | Metal      |
| :------------- | ----------: | ---------: |
| Geekbench     |        4193 |        4035 |
</details>

# CONTACT

- Email: ryebread931@gmail.com
- Discord: rye#7685
- Telegram: @rye_1

# Credits

- [Apple](https://www.apple.com) for macOS.
- [Acidanthera](https://github.com/acidanthera) for all the kexts/utilities that they made.
- [Rehabman](https://github.com/RehabMan) and [Daliansky](https://github.com/daliansky) for the patches and guides and kexts.
- [Dortania](https://github.com/dortania) for for the OpenCore Install Guide.
