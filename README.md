<h1>SVT14126CVS OpenCore EFI - macOS 10.15 and 11 (not sure about 12 tho)</h1>
<h2>Here you can download the EFI of QuanTrieuPCYT's new hackintosh PC! (basically a SVT14126CVS without a screen, so if you want to use this EFI for your hackintosh please change framebuffers and shits in the config.plist)</h2>
<h2>OpenCore 0.6.4 bootloader, with OpenCanopy Big Sur and Boot Chime!</h2>
<p>Designed for Big Sur, Catalina and older please change SMBIOS.</p>

You want sidecar support? Go get <a href="https://github.com/hieplpvip/SidecarEnabler">Sidecar Enabler</a>!

If you have a Sony VAIO SVT14 with a Z40UL.MB motherboard, you can use this EFI! But you will need to change the followings:
* Update your BIOS
* Add Kexts for your Camera and your ELAN touch screen.
* Patch iGPU (change AAPL,ig-platform-id to 03006601 for 1366x768, 04006601 and add some parameters for 1600x900 or higher)
* Change SMBIOS information

![126064336-a2d9b5c0-40fd-40bc-9083-57be133c8f25.png](https://user-images.githubusercontent.com/73286927/126064336-a2d9b5c0-40fd-40bc-9083-57be133c8f25.png)

**Hackintosh (connected to an HDMI TV) next to a 13-inch Macbook Pro 2019. Both running macOS Big Sur**

![image](https://user-images.githubusercontent.com/73286927/126935674-246a37cc-b600-4109-b10f-f924a8f350f8.png)

**Same Hackintosh running macOS Catalina 10.15.6**

<br>

This machine is basically an SVT14126CVS without a keyboard, a touchpad and a screen (pretty much like a Desktop)
Specs:
* CPU: Intel Core i5-3337U (Ivy Bridge Mobile)
* RAM: 8GB DDR3
* GPU: Intel HD Graphics 4000
* Motherboard: Z40UL.MB (mainboard of the SVT14 VAIOs, mine is SVT14126CVS)
* SSD: Kingston V300 120GB
* Wireless Card: AR9485
* Ethernet: RTL8111
* HDMI as screen output (no LVDS).

## ✅ Whats workin'
* Graphics acceleration (Intel HD Graphics 4000)
* USB 2.0 and 3.0 (all)
* Ethernet (using old kext)
* Audio
* SD Card slot (partially, read the **Not workin'** section)
* Sleep & Wake (now works with USB mapping)
* iServices (using **this guide: https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html**)
* Keyboard
* Touchpad
* Webcam
* Touchscreen (ELAN)
## ❌ Not workin'
* CPU Power Management (not something important but will be fixed in a future release)
* SD Card hotplugging and after sleep (will be fixed in a later release)
* **You tell me**

Have fun hackintoshing!
<3 from QuanTrieuPCYT
