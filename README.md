# Asus ROG Strix B550-I + Ryzen 9 5900X + RX 6800

- OpenCore ver 0.8.4
- MacPro7,1
- Monterey 12.6

Work in progress, can’t get Installer past grey screen after choosing language. Mouse can be moved, but nothing happens.

## Current hardware

Powerful and near-silent even under full CPU load.

- Asus [ROG Strix B550-I Gaming](https://rog.asus.com/us/motherboards/rog-strix/rog-strix-b550-i-gaming-model/) motherboard
- AMD [Ryzen 9 5900X](https://www.amd.com/en/products/cpu/amd-ryzen-9-5900x) CPU
- EK [Basic 240](https://www.ekwb.com/shop/ek-aio-basic-240) AIO
- AMD [RX 6800](https://www.amd.com/en/products/graphics/amd-radeon-rx-6800) graphics card.
- Corsair [Vengeance LPX](https://www.corsair.com/us/en/Categories/Products/Memory/VENGEANCE-LPX/p/CMK32GX4M2D3200C16) 32 GB (2 x 16 GB) DDR4 3200MHz CL16
- 2 × WD [Blue SN570](https://www.westerndigital.com/products/internal-drives/wd-blue-sn570-nvme-ssd#WDS100T3B0C) 1TB NVMe SSD
- Corsair [SF600 Platinum](https://www.corsair.com/us/en/Categories/Products/Power-Supply-Units/Power-Supply-Units-Advanced/SF-Series/p/CP-9020182-NA) SFX PSU
- Noctua [NF-A12x15](https://noctua.at/en/products/fan/nf-a12x15-pwm) case fan as the bottom exhaust
- Nouvolo [Steck 1.1](https://www.nouvolo.com/pages/steck) SFF case with top expansion stack

### BIOS

Version 2803

- Fast Boot: `Disabled`
- CSM: `Disabled`
- Above 4G Decoding: `Enabled`
- Resizable Bar Support: `Enabled`
- PCIe slot speed: `Gen3`
- XMP Profile activated (D.O.C.P.)

## Usage

1. [Update `PlatformInfo/Generic` stuff](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#generate-a-new-serial) with your own, inside `config.plist`
2. Use your Ethernet’s MAC address for `ROM` value, as explained in the Dortania guide. Don’t leave it as all 0s.

## Notes

Use at your own risk. 

- All `.efi` drivers and `.kext` are `-RELEASE` builds from the respective packages. 
- OpenCanopy (GUI boot menu) is up and running.
- I don’t boot Windows 10 using OC, thus I can’t guarantee it will work. I have Win 10 installed on separate SSD and switch using Boot Menu.

**Don’t ask me for help.** Sorry but this stuff is finicky and infuriatingly detailed that every little mis-step can be a proper headache. This is why [Dortania](https://dortania.github.io) advises to not reuse anyone’s EFI.  

Ask [on reddit](https://www.reddit.com/r/hackintosh/) and the [discord server](https://discord.gg/Wxam8aH).

Good luck.

## Give back

If you found this code useful, please consider [buying me a coffee](https://www.buymeacoffee.com/radianttap) or two. ☕️😋
