# Asus ROG Strix B550-I · Ryzen 5x00 · Radeon 6x00

- OpenCore ver 0.9.6
- MacPro7,1
- Sonoma 14.1.1

*Use at your own risk.* Nothing is guaranteed, even if you use exactly the same hardware as me.

You may use this EFI as example but be prepared to dive way deeper than you hoped. It’s always advisable to build your own EFI from scratch, [following the guide](https://dortania.github.io/OpenCore-Install-Guide/) —  then you’ll have an idea how things work and how to ask for help in proper channels:
- [Discord server](https://discord.gg/Wxam8aH)
- AMD-OSX [forums](https://forum.amd-osx.com)

Most importantly — doing stuff step by step will give you knowledge how to act on given help and hints.

Good luck.


## Current hardware

- Asus [ROG Strix B550-I Gaming](https://rog.asus.com/us/motherboards/rog-strix/rog-strix-b550-i-gaming-model/) motherboard
- AMD [Ryzen 7 5700X](https://www.amd.com/en/products/cpu/amd-ryzen-7-5700x) CPU
- AMD [RX 6800](https://www.amd.com/en/products/graphics/amd-radeon-rx-6800) graphics card.
- Corsair [Vengeance LPX](https://www.corsair.com/us/en/Categories/Products/Memory/VENGEANCE-LPX/p/CMK32GX4M2D3200C16) 32 GB (2 x 16 GB) DDR4 3200MHz CL16
- WD [Black SN850X](https://www.westerndigital.com/en-il/products/internal-drives/wd-black-sn850x-nvme-ssd#WDS200T2X0E) 2TB NVMe SSD
- WD [Black SN770](https://www.westerndigital.com/en-il/products/internal-drives/wd-black-sn770-nvme-ssd#WDS100T3X0E) 1TB NVMe SSD
- Intel AX200 Wi-Fi / Bt card is already included on the motherboard.

Note: it’s fairly easy to switch between Ryzen 5000 CPUs, just carefully update the `Replace` value in first 4 `Kernel/Patch` entries, as [per AMD OSX Vanilla repo](https://github.com/AMD-OSX/AMD_Vanilla).

You can use any of these cards: Radeon 5500 XT, 5700 XT, 6600 XT, 6800, 6800 XT, 6900 XT — all are natively supported and none require any extra setup to do.

### BIOS

Version 2803

- Fast Boot: `Disabled`
- CSM: `Disabled`
- Above 4G Decoding: `Enabled`
- Resizable Bar Support: `Enabled`
- PCIe slot speed: `Auto`
- XMP Profile activated (D.O.C.P.)

### Stuff you need to do

1. Update PlatformInfo/Generic stuff with your own, inside `config.plist`. Generate [appropriate values](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#generate-a-new-serial) for `MLB` (also called Board Serial), `SystemSerialNumber` and `SystemUUID`.
2. Use your Ethernet’s MAC address for `ROM` value, as [explained](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#choose-a-mac-address) in the Dortania guide.

Don’t leave these settings as all zeros, iCloud and other Apple services will not work.

## Status, stability

- Intel Wi-Fi drivers I am using ([AirportItlwm](https://github.com/OpenIntelWireless/itlwm/releases) 2.3.0 alpha) don’t support niceties like AirDrop. On the other hand, Wi-Fi speed is way, way better than with common replacements like BCM94360NG thus I’m thinking the trade-off is worth it.
- Basic iCloud is working, file sync etc.
- Messages / Facetime won't login, for now.
- Sleep is not working.

Otherwise the build is pretty much perfect and performance is great.

## Give back

If you found this code useful, please consider [buying me a coffee](https://www.buymeacoffee.com/radianttap) or two. ☕️😋
