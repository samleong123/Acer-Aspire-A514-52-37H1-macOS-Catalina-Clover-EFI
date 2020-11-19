# Acer# Acer Aspire A514-52-37H1 macOS Catalina Clover EFI

#### macOS Catalina Version : 10.15.7
#### Clover Version : v2.5k r5120
#### Special thanks to [Daliansky](https://github.com/daliansky)

### Currently knew problem : 
- HDMI wont work
- Headphone Jack wont work
- AppleALC unable inject any layout ID on ALC256
- VoodooHDA used and Internal Mic is working but contain a little bit crack sound
- Sometimes IO80211 will crashed and caused a kernel panic , just reboot and usually will solve it
- DRM Content wont work
- FN Keys for Brightness wont work , only Volume Mute / Up / Down working


## 19-11-2020 1300
- Added support for trackpad (VoodooI2C) with correct hotpatch and SSDT
    - Remove broken brightness control that will conflict with Trackpad SSDT
    - Added new brightness control 

## 19-11-2020 0900
- Added new brightness control
  - Update : 19-11-2020 : This brightness control will conflict with Trackpad SSDT , removed and added another new brightness control patch

## 18-11-2020 2200
- Added support for Intel AX201 with Airportitlwm.kext

## 18-11-2020 1800
- Added EFI from [DalianSky Catalina 10.15.7 Image](http://blog.daliansky.net/macOS-Catalina-10.15.7-19H2-Release-version-with-Clover-5122-original-image-Double-EFI-Version-UEFI-and-MBR.html)
