# Asus ROG Strix B550-I + Ryzen 7 5700X + RX 6800

- OpenCore ver 0.8.7
- MacPro7,1
- Monterey 12.6.2

## Current hardware

- Asus [ROG Strix B550-I Gaming](https://rog.asus.com/us/motherboards/rog-strix/rog-strix-b550-i-gaming-model/) motherboard
- AMD [Ryzen 7 5700X](https://www.amd.com/en/products/cpu/amd-ryzen-7-5700x) CPU
- AMD [RX 6800](https://www.amd.com/en/products/graphics/amd-radeon-rx-6800) graphics card.
- Corsair [Vengeance LPX](https://www.corsair.com/us/en/Categories/Products/Memory/VENGEANCE-LPX/p/CMK32GX4M2D3200C16) 32 GB (2 x 16 GB) DDR4 3200MHz CL16
- WD [Black SN850X](https://www.westerndigital.com/en-il/products/internal-drives/wd-black-sn850x-nvme-ssd#WDS200T2X0E) 2TB NVMe SSD
- WD [Black SN770](https://www.westerndigital.com/en-il/products/internal-drives/wd-black-sn770-nvme-ssd#WDS100T3X0E) 1TB NVMe SSD
- Corsair [SF600 Platinum](https://www.corsair.com/us/en/Categories/Products/Power-Supply-Units/Power-Supply-Units-Advanced/SF-Series/p/CP-9020182-NA) SFX PSU
- Noctua [NF-L12 Ghost S1](https://noctua.at/en/nh-l12-ghost-s1-edition) CPU cooler
- Louqe [Ghost S1 Mk3](https://www.louqe.com/portfolio/ghost-s1/) case

Note: it’s fairly easy to switch between Ryzen 5000 CPUs, just carefully update the `Replace` value in first 3 `Kernel/Patch` entries, as [per AMD OSX Vanilla repo](https://github.com/AMD-OSX/AMD_Vanilla).

### BIOS

Version 2803

- Fast Boot: `Disabled`
- CSM: `Disabled`
- Above 4G Decoding: `Enabled`
- Resizable Bar Support: `Enabled`
- PCIe slot speed: `Auto`
- XMP Profile activated (D.O.C.P.)

## Usage

1. [Update `PlatformInfo/Generic` stuff](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#generate-a-new-serial) with your own, inside `config.plist`
2. Use your Ethernet’s MAC address for `ROM` value, as explained in the Dortania guide. Don’t leave it as all 0s.

## Notes

*Use at your own risk.* Nothing is guaranteed, even if you use exactly the same hardware as me.

You may use this EFI as example but be prepared to dive way deeper than you hoped. It’s always advisable to build your own EFI from scratch, [following the guide](https://dortania.github.io/OpenCore-Install-Guide/) —  then you’ll have an idea how things work,  how to ask for help in proper channels:
- [on Reddit](https://www.reddit.com/r/hackintosh/)
- [Discord server](https://discord.gg/Wxam8aH)
- AMD-OSX [forums](https://forum.amd-osx.com)

Most importantly — doing stuff step by step will give you knowledge how to act on given help and hints.

Good luck.

## Give back

If you found this code useful, please consider [buying me a coffee](https://www.buymeacoffee.com/radianttap) or two. ☕️😋
