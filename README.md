Here you can download the EFI of QuanTrieuPCYT's new hackintosh PC!
OpenCore 0.6.4 bootloader, with OpenCanopy Big Sur and Boot Chime!
Designed for Big Sur, Catalina and older please change SMBIOS.
If you have a Sony VAIO SVT14 with a Z40UL.MB motherboard, you can use this EFI! But you will need to change the followings:
- Add Kexts for your Camera and your ELAN touch screen.
- Patch iGPU (change AAPL,ig-platform-id to 03006601 for 1366x768, 04006601 and add some parameters for 1600x900 or higher)
- Change SMBIOS information

Specs:
CPU: Intel Core i5-3337U (Ivy Bridge Mobile)
RAM: 8GB DDR3
GPU: Intel HD Graphics 4000
Motherboard: Z40UL.MB (mainboard of the SVT14 VAIOs, mine is SVT14126CVS)
SSD: Kingston V300 120GB
Wireless Card: AR9485

Everything is working on this PC running macOS except:
- The RTS5209 Realtek PCIe SD Card Reader is not functioning properly. You will need to insert the card before booting so macOS can recognize your card. ProDuo cards is not tested, if you can please test it for me.
- Bluetooth is not working on AR9485 (since High Sierra maybe). Wi-FI is working but with a really slow speed.
- Apple DRM contents (According to OpenCore Instal Guide, DRM is broken on iGPU-only PCs)

Have fun!
<3 from QuanTrieuPCYT
and thanks valiantarchy lmao
