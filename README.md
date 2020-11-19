# Acer Aspire A514-52-37H1 macOS Catalina Clover EFI

#### macOS Catalina Version : 10.15.7
#### Clover Version : v2.5k r5120
#### Special thanks to [Daliansky](https://github.com/daliansky)
#### EFI Download : [Click here](https://github.com/samleong123/Acer-Aspire-A514-52-37H1-macOS-Catalina-Clover-EFI/releases)

### Specifications
- Intel i3-10110u Dual Core Processor [WORKING WITHOUT SPOOF]
- Intel UHD 620 (NO DGPU)[ VRAM SET ON 2048MB SINCE 19-11-2020 0900] [VRAM ON 1536MB : 18-11-2020 2200] [HDMI NOT WORKING] [IF YOU HAVE ANY SOLUTION TO SOLVE THIS PLEASE COMMIT TO THIS REPO]
- Sound : Realtek ALC256 [ FULLY WORKING SINCE 19-11-2020 2210] 
- Trackpad : I2C Synaptics [WORKING SINCE 19-11-2020 1300]
- 2 x USB 3.1 Gen 1 A Port [WORKING] [5GBPS FULL SPEED]
- 1 x USB 3.1 Gen 1 C Port [WORKING] [5GBPS FULL SPEED]
- 1 x USB 2.0 A Port [WORKING] [480MBPS FULL SPEED]
- 1 x 3.5mm Headphone Jack [WORKING SINCE 19-11-2020 2210] [[ComboJack](https://github.com/hackintosh-stuff/ComboJack) needed for headphones jack working!]
- 1 x RJ45 Realtek RTL8111 1GBPS [WORKING]
- 1 x HDMI port [NOT WORKING] [IF YOU HAVE ANY SOLUTION TO SOLVE THIS PLEASE COMMIT TO THIS REPO]
- 2.4GHz & 5GHz WiFi & Bluetooth : INTEL AX201 [WORKING] [RUNNING ONLY AT 20MHZ ON 2.4GHZ & 5GHZ] THANKS TO [zxystd](https://github.com/zxystd)!
- 1 x HD User Facing (Connected through USB) [WORKING]

### Screenshots 
- Intel AX201 2.4GHz & 5GHz & Bluetooth Work!
- Trackpad Work!
- Youtube 4K 2160P work perfectly!
![image](https://raw.githubusercontent.com/samleong123/Acer-Aspire-A514-52-37H1-macOS-Catalina-Clover-EFI/main/Screenshots/Screenshot%202020-11-19%20at%203.08.20%20PM.png)


![image](https://raw.githubusercontent.com/samleong123/Acer-Aspire-A514-52-37H1-macOS-Catalina-Clover-EFI/main/Screenshots/Screenshot%202020-11-19%20at%203.08.45%20PM.png)


![image](https://raw.githubusercontent.com/samleong123/Acer-Aspire-A514-52-37H1-macOS-Catalina-Clover-EFI/main/Screenshots/Screenshot%202020-11-19%20at%203.09.50%20PM.png)


![image](https://raw.githubusercontent.com/samleong123/Acer-Aspire-A514-52-37H1-macOS-Catalina-Clover-EFI/main/Screenshots/Screenshot%202020-11-19%20at%203.13.41%20PM.png)

### Currently knew problem : 
- HDMI wont work
- Sometimes IO80211 will crashed and caused a kernel panic , just reboot and usually will solve it
- DRM Content wont work
- FN Keys for Brightness wont work , only Volume Mute / Up / Down working

## 19-11-2020 2200
- Added layout-id to 13 in boot args [AUDIO FINALLY WORK] 
  - [ComboJack](https://github.com/hackintosh-stuff/ComboJack) needed for headphones jack working 
  - For [ComboJack](https://github.com/hackintosh-stuff/ComboJack) , VerbStub.kext already loaded inside EFI/Clover/Kexts/Other , to install [ComboJack](https://github.com/hackintosh-stuff/ComboJack) , simply run install.sh that inside ComboJack_Installation folder , you can also replace the latest VerbStub.kext along with the install.sh file into EFI/Clover/Kexts/Other.

## 19-11-2020 1300
- Added support for trackpad (VoodooI2C) with correct hotpatch and SSDT
    - Remove broken brightness control that will conflict with Trackpad SSDT
    - Added new brightness control 
    - VRAM set to 2048MB

## 19-11-2020 0900
- Added new brightness control
  - Update : 19-11-2020 : This brightness control will conflict with Trackpad SSDT , removed and added another new brightness control patch
  - VRAM set to 2048MB

## 18-11-2020 2200
- Added support for Intel AX201 with Airportitlwm.kext
- VRAM should remain at 1536MB

## 18-11-2020 1800
- Added EFI from [DalianSky Catalina 10.15.7 Image](http://blog.daliansky.net/macOS-Catalina-10.15.7-19H2-Release-version-with-Clover-5122-original-image-Double-EFI-Version-UEFI-and-MBR.html)
- If use original EFI from [DalianSky Catalina 10.15.7 Image](http://blog.daliansky.net/macOS-Catalina-10.15.7-19H2-Release-version-with-Clover-5122-original-image-Double-EFI-Version-UEFI-and-MBR.html) will caused VRAM at 5MB / 7MB display only.
