<h1>SVT14126CVS OpenCore EFI</h1>
<h2>Here you can download the EFI of QuanTrieuPCYT's new hackintosh PC! (basically a SVT14126CVS without a screen, so if you want to use this EFI for your hackintosh please change framebuffers and shits in the config.plist)</h2>
<h2>OpenCore 0.6.4 bootloader, with OpenCanopy Big Sur and Boot Chime!</h2>
<p>Designed for Big Sur, Catalina and older please change SMBIOS.</p>
![https://user-images.githubusercontent.com/73286927/126064336-a2d9b5c0-40fd-40bc-9083-57be133c8f25.png](https://user-images.githubusercontent.com/73286927/126064336-a2d9b5c0-40fd-40bc-9083-57be133c8f25.png)


You want sidecar support? Go get <a href="https://github.com/hieplpvip/SidecarEnabler">Sidecar Enabler</a>!

If you have a Sony VAIO SVT14 with a Z40UL.MB motherboard, you can use this EFI! But you will need to change the followings:
- Add Kexts for your Camera and your ELAN touch screen.
- Patch iGPU (change AAPL,ig-platform-id to 03006601 for 1366x768, 04006601 and add some parameters for 1600x900 or higher)
- Change SMBIOS information

Lemme tell you guys a story...
<p>I had an old laptop, which is badly smashed (Sony VAIO SVT14126CVS).</p>
<p>I pulled the mainboard out, removed the screen and the keyboard. Now it's a real Desktop PC.</p>
<p>Display output using HDMI. VGA is working (tested with my old 1280x1024 VGA display) but not under macOS.</p>

Specs:
- CPU: Intel Core i5-3337U (Ivy Bridge Mobile)
- RAM: 8GB DDR3
- GPU: Intel HD Graphics 4000
- Motherboard: Z40UL.MB (mainboard of the SVT14 VAIOs, mine is SVT14126CVS)
- SSD: Kingston V300 120GB
- Wireless Card: AR9485
- LAN Controller: RTL8111
- HDMI as screen output (no LVDS).

Everything is working on this PC running macOS except:
- Unstable FireVault upport.
- The RTS5209 Realtek PCIe SD Card Reader is not functioning properly (hot-plugging is not possible). You will need to insert the card before booting so macOS can recognize your card. And also, after putting your PC into sleep mode and wake it up again, the SD Card Reader no longer functions, so if you want to use the SD Card continuously please don't put the PC into sleep. ProDuo cards is not tested, if you can please test it for me.
- Bluetooth is not working on AR9485 (since High Sierra maybe). Wi-FI is working but with a really slow speed.
- Apple DRM contents (According to OpenCore Install Guide, DRM is broken on iGPU-only PCs)

Have fun!
<3 from QuanTrieuPCYT
and thanks valiantarchy lmao
