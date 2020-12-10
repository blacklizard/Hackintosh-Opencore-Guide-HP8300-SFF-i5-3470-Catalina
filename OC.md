# OpenCore EFI

Download OpenCore **RELEASE** from [here](https://github.com/acidanthera/OpenCorePkg/releases/latest)


## ACPI 
- SSDT-PM.aml `Generate your own PM using https://github.com/Piker-Alpha/ssdtPRGen.sh` - Not needed for USB installer
- SSDT-EC.aml
- SSDT-HPET.aml

## Driver
- [HfsPlus.efi](https://github.com/acidanthera/OcBinaryData/raw/master/Drivers/HfsPlus.efi)
- OpenRuntime.efi - Included in OpenCore package

## Kext - Make sure to download RELEASE version
- [Lilu.kext](https://github.com/acidanthera/Lilu/releases/latest)
- [VirtualSMC.kext](https://github.com/acidanthera/VirtualSMC/releases/latest)
- [WhateverGreen.kext](https://github.com/acidanthera/WhateverGreen/releases/latest)
- [AppleALC.kext](https://github.com/acidanthera/AppleALC/releases/latest)
- [IntelMausi.kext](https://github.com/acidanthera/IntelMausi/releases/latest)
- USBPorts.kext - Use the one included in this repo
- SMCProcessor.kext - Included in VirtualSMC package
- SMCSuperIO.kext - Included in VirtualSMC package

## Tools
- [modGRUBShell.efi](https://github.com/datasone/grub-mod-setup_var/releases/download/1.1/modGRUBShell.efi)
- OpenShell.efi - Included in OpenCore package
- ResetSystem.efi - Included in OpenCore package
- CleanNvram.efi - Included in OpenCore package

## config.plist

- Use `config.plist` for internal boot disk.

## EFI Folder Structure
### SSD/NVME/HDD
```
EFI
├── BOOT
│   └── BOOTx64.efi
└── OC
    ├── ACPI
    │   ├── SSDT-PM.aml
    │   ├── SSDT-EC.aml
    │   └── SSDT-HPET.aml
    ├── Bootstrap
    │   └── Bootstrap.efi
    ├── Drivers
    │   ├── HfsPlus.efi
    │   └── OpenRuntime.efi
    ├── Kexts
    │   ├── AppleALC.kext
    │   ├── IntelMausi.kext
    │   ├── Lilu.kext
    │   ├── SMCProcessor.kext
    │   ├── SMCSuperIO.kext
    │   ├── USBPorts.kext
    │   ├── VirtualSMC.kext
    │   └── WhateverGreen.kext
    ├── OpenCore.efi
    ├── Tools
    │   ├── CleanNvram.efi
    │   ├── OpenShell.efi
    │   ├── ResetSystem.efi
    │   └── modGRUBShell.efi
    └── config.plist

```
