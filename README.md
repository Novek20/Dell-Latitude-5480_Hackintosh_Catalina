# Dell Latitude 5480 Hackintosh EFI - macOS 10.15
**Can be used for the Dell Latitude 5280/5580 and the Dell Precision 3520 as well (w/ some modifications)**

OpenCore bootloader for stability.

**NOTE:**
* Use [**one-key-hidpi**](https://github.com/xzhih/one-key-hidpi) to get HiDPI support in macOS
* Please [**disable your CFG Lock**](/Disable_CFG_Lock.md) and [**adjust your DVMT**](/Adjusting_DVMT.md).

![Screen-Shot-2023-11-20-at-2](https://github.com/Novek20/Dell-Latitude-5480_Hackintosh_Catalina/assets/47246274/31af2ded-e310-458c-94f1-172447423db8)


**Model: Dell Latitude 5480**
- **CPU:** Intel® Core™ i5-7300U
- **GPU:** Intel® HD Graphics 620
- **RAM:** 8GB DDR4 2133MHz
- **Ethernet:** Intel® Ethernet I219-LM
- **Wi-Fi:** Intel® Dual Band Wireless-AC 8265
- **Sound Card:** ALC256 (layout-id `69` with [**ALC256.kext**](https://github.com/ic005k/ALC256))
- **Trackpad:** AlpsAlpine U1 Dual I2C Touchpad (`0x120b`)
- **SD Card Reader:** Realtek RTS525A
- **Internal Display:** 1920x1080 Full HD Screen
- **Runs Big Sur with Monterey perfectly 👌**

## ✅ Whats workin'
* Graphics acceleration (Intel® HD Graphics 620)
* Dual Display with VGA, USB-C and HDMI ports.
* All USB ports (3x USB 3.0, 1x USB-C)
* Ethernet
* Audio (using [**ALC256.kext with `layout-id` set to `69`**](https://github.com/ic005k/ALC256))
* SD Card slot (using [**RealtekCardReader**](https://github.com/0xFireWolf/RealtekCardReader) and [**RealtekCardReaderFriend**](https://github.com/0xFireWolf/RealtekCardReaderFriend/))
* Sleep & Wake with Lid (now works with USB mapping and [**GPRW and UPRW Instant Wake Patch**](https://dortania.github.io/OpenCore-Post-Install/usb/misc/instant-wake.html))
* CPU Power Management
* iServices (using **this guide: https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html**)
* SMBUS
* Microphone
* Multi gestures touchpad (thanks to [**Juico's AlpsT4USB - which is now blankmac's AlpsHID**](https://github.com/blankmac/AlpsHID)!)
* Front Camera
* Boot Chime
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
* [cholonam](https://github.com/cholonam), [syscl](https://github.com/syscl) and [sinetek](https://github.com/sinetek) for [**Sinetek-rtsx**](https://github.com/cholonam/Sinetek-rtsx) (thanks for bringing my SD Card reader back to life)
* [0xFireWolf](https://github.com/0xFireWolf) for [**RealtekCardReader**](https://github.com/0xFireWolf/RealtekCardReader) and [**RealtekCardReaderFriend**](https://github.com/0xFireWolf/RealtekCardReaderFriend/) (basically a better version of [**Sinetek-rtsx**](https://github.com/cholonam/Sinetek-rtsx))
* And special thanks to [**Văn Hùng Nguyễn**](https://github.com/vanhung4499) (vanhung4499) for helping me with the touchpad fix (the hardest part)
