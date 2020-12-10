# BIOS Configuration

BIOS version: `00.03.06 Rev.A`

- Load Optimized Defaults
- Storage -> SATA emulation -> AHCI
- Storage -> Removable Media Boot -> Enabled
- Security -> Network Boot -> Disabled
- Secure Boot -> Legacy Support: Disabled
- Secure Boot -> Secure Boot: Disabled
- Secure Boot -> Fast Boot - Enabled

## Hidden BIOS setting
This setting can be modified using [modGRUBShell.efi](https://github.com/datasone/grub-mod-setup_var/releases/download/1.1/modGRUBShell.efi)
⚠️: These offset are only valid for the specific firmware version! Do not try to execute these commands on a different firmware! 
The modified variables will reset itself when you restore / revert to optimised defaults. 
Everytime BIOS is reset, you will need to reconfigure the hidden setting or else you will not be able to boot, you have been warned

#### Required setting
- Disable CFG Lock 

| Firmware Version | Command              |
|------------------|----------------------|
| 00.03.06 Rev.A     |`TBD`|

