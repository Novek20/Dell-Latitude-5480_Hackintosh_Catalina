# Dell Latitude 5480 Hackintosh EFI - macOS 11 and 12
**Introducing my new hack: Dell Latitude 5480 running macOS!**

OpenCore bootloader for stability.

![screenshot with neofetch](https://user-images.githubusercontent.com/73286927/134603078-0e84dd30-b772-41c0-83b8-c9c946951edd.png)
**Running fine on macOS Big Sur. Monterey should work, but you'll need to update your Wi-Fi kext.**

![Dual Display - VGA](https://user-images.githubusercontent.com/73286927/134603760-0973d4ed-5a09-480b-8e1b-0e6785ccb6e9.jpg)
**Dual Display with VGA port** (somehow it worked)

![Dual Display - USB-C](https://user-images.githubusercontent.com/73286927/134603810-fbbc3409-e3d5-409d-a0c5-0a340c62ee3f.jpg)
**Dual Display with USB-C hub** (HDMI also works and it outputs the same image)

## Laptop Specs
![the laptop itself](https://user-images.githubusercontent.com/73286927/134605704-947a77cf-4f3a-4b4c-ad7b-e76d07806fd0.jpg)

**Model: Dell Latitude 5480**
- **CPU:** Intel® Core™ i5-7200U
- **GPU:** Intel® HD Graphics 620
- **RAM:** 8GB/16GB DDR4 2133MHz
- **Ethernet:** Intel® Ethernet I219-LM
- **Wi-Fi:** Intel® Dual Band Wireless-AC 8265
- **Sound Card:** ALC256 (layout-id `21`)
- **Trackpad:** Alps I2C HID Trackpad (DLL07A7)
- **SD Card Reader:** Realtek RTS525A
- **Internal Display:** 1920x1080 Full HD Screen
- **Runs Big Sur perfectly, haven't tried Monterey yet**

## ✅ Whats workin'
* Graphics acceleration (Intel® HD Graphics 620)
* Dual Display with VGA, USB-C and HDMI ports.
* USB 3.0 ports and USB-C
* Ethernet
* Audio (ALC256 with VerbStub, or you can use [**this kext with `layout-id` set to `69` cuz it also works**](https://github.com/ic005k/ALC256)
* SD Card slot (macOS detects it as a normal USB 2.0 device, not a PCI-E card reader so it will work just fine)
* Sleep & Wake with Lid (now works with USB mapping)
* CPU Power Management (fixed in 1.1 release)
* iServices (using **this guide: https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html**)
* SMBUS
* Microphone
* Touchpad (just basic scrolling and click functions)
## ❌ Not workin'
* DRM (not possible on iGPU-only hacks)
* Handoff, AirDrop and Apple Watch Unlock (until you use a Broadcom Wi-Fi card)
* **You tell me**

## Credits
* [Apple](https://apple.com) for [**macOS**](https://apple.com/macos)
* [acidanthera](https://github.com/acidanthera) for [**OpenCore**](https://github.com/acidanthera/OpenCorePkg), [**Lilu**](https://github.com/acidanthera/Lilu), [**WhateverGreen**](https://github.com/acidanthera/WhateverGreen) and [**AppleALC**](https://github.com/acidanthera/AppleALC)
* [Dortania](https://dortania.github.io) for [**OpenCore Install Guide**](https://dortania.github.io/OpenCore-Install-Guide)
* [RehabMan](https://github.com/RehabMan) for [**USBInjectAll**](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/) (without this kext i will not be able to map USB)
* [headkaze](https://github.com/headkaze) for [**Hackintool**](https://github.com/headkaze/Hackintool)
* [NVIDIA](https://nvidia.com) for [**NVIDIA Web Drivers**](https://www.tonymacx86.com/nvidia-drivers)
* And special thanks to [**Văn Hùng Nguyễn**](https://github.com/vanhung4499) (vanhung4499) for helping me with the touchpad fix (the hardest part)
