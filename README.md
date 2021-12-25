# X270-Monterey-OpenCore
EFI for Monterey OpenCore Hackintosh

# Introduction
While Monterey is brand spanking new, that also presents problems for those looking to upgrade.
If you're new to hackintosh, prefer stability and you're 100% dependent on the touchpad, I would not recommend upgrading but rather staying on something like Big Sur. There are a lot of good repos for this, including [one with a fully functioning touchpad/buttons (my fork)](https://github.com/aerowa/Lenovo-X270-Hackintosh-OpenCore) or [michaeldigiacomi's X270](https://github.com/michaeldigiacomi/Lenovo-X270-Hackintosh-OpenCore)

But honestly, that's probably the biggest downside.
![About](images/about.png)

# Tested OS
- [x] macOS Monterey (12.1)

![X270](images/screen.png)

# Hardware
- ThinkPad X270
- i7-7500U
- HD 620 iGPU
- 1TB SSD
- 16GB DDR4 RAM
- Intel AC 8260 (Standard WiFi/BT)
- Standard 1080p IPS screen

# BIOS
- Ver. 
### Settings
<b>Security</b>
- `Security Chip` **Disabled**
- `Memory Protection -> Execution Prevention` **Enabled**
- `Virtualization -> Intel Virtualization Technology` **Enabled**
- `Virtualization -> Intel VT-d Feature` **Enabled**
- `Anti-Theft -> Computrace -> Current Setting` **Disabled**
- `Secure Boot -> Secure Boot` **Disabled**
- `Intel SGX -> Intel SGX Control` **Disabled**
- `Device Guard` **Disabled**

<b>Startup</b>
- `UEFI/Legacy Boot` **UEFI Only**
- `CSM Support` **No**

# Working
- [x] WiFi (Airportitlwm)
- [x] Integrated Camera
- [x] AppleID Services (FaceTime, iMessage, App Store)
- [x] HD 620 Graphics
- [x] CPU Power Management
- [x] Battery Management
- [x] Sleep & Resume (Not lid)
- [x] USB Ports
- [x] Audio (+ jack)
- [x] Bluetooth
- [x] Keyboard (including FN)
- [x] Touchpad Gestures
- [x] Shutdown
- [x] DRM Support

# Not tested
- HDMI
- SD Reader
- Fingerprint reader
- Sidecar
- AirDrop

# Not working
- Physical Touchpad buttons
- Sleep/Wake (lid)

# Notes
- WiFi is underperforming, this is pretty standard for all Intel WiFi cards using itlwm
- To use AppleID services remember to change SMBIOS
- Bluetooth injector can result in a slow boot (looks like bootloop - but isn't), disable if not used

# Other
- OpenCore ver. 0.7.6
- [corpnewt - MountEFI & GenSMBIOS](https://github.com/corpnewt)
- [OpenCore](https://dortania.github.io/OpenCore-Install-Guide/)

# Thank you
- [michaeldigiacomi's X270](https://github.com/michaeldigiacomi/Lenovo-X270-Hackintosh-OpenCore) (Big Sur EFI - i5 series)
- [taida2203's fork](https://github.com/taida2203/Lenovo-X270-Hackintosh-OpenCore) (Big Sur EFI - i7 compatibility)
