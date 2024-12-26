# HP-au146tx-Sequoia-EFI
This is an OPENCORE efi for HP Pavilion au146tx to boot into macOS Sequoia.

## Warning
1. This efi could also work for Sonoma, but stability untested.
2. There's no SMCBatteryManager.kext as I had remove the battery off of my laptop. Add into both folders and plist if needed.
3. After installation set SMBIOS to MacBookPro14,1 and generate a set of S/N, MLB and UUID yourself.
4. I managed to unlock CFGlock but still reserved 2 boxes checked for you. If you unlock too, disable them. If you don't know what this is, just ignore.
4. You might need to build your own USBMap kext.
5. Deploy at your own risk!

## Specsheet
- Intel(R) Core(TM) i5-7200U @2.5GHz
- Intel HD Graphics 620, Total Shared Mem=4038MiB
- Realtek ALC295 [C1], alcid=77
- Intel(R) Dual Band Wireless-AC 3168 NGW
- Realtek RTL8139/810x Fast Ethernet Adapter | RTL810xE (100Mbps)
- Synaptics SMBus TouchPad (PS/2 in linux)
- Standard PS/2 Keyboard

## What won't work
- dGPU NV GTX 940MX
- Internal Wi-Fi, but itlwm is usable as ethernet, You would need Heliport for now.
- The amazing chime at startup
- A tray-icon of the SDXC reader, can be closed manually or disable in ACPI.

## Credits
- dortania.github.io
- github.com/acidanthera
- github.com/yusufklncc, a lot.
