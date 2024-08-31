![Screenshot 2567-08-31 at 09 53 23](https://github.com/user-attachments/assets/3057dadd-a696-4382-bf8b-9e586719a05c)

# OCLP 1.5.0 - macOS Ventura 13.6.9 - Lenovo Z50-70 Type 80E7 59422137

macOS 13 Ventura is **NOT** supported **NATIVELY** for Haswell system (2013 Intel 4th-gen core cpu) if you want **STABLE** os to use please head to my other repository [OpenCore Lenovo Z50-70](https://github.com/JuicerV3/Opencore-Monterey-Z50-70).

```
* I am not responsible for any damage done to your device. Use at your own risk.
* Please do some research if you concerns about features included in this EFI.
* Before continuing, you are choosing to make these modifications yourself
* if any thing goes wrong, it is your responsible for the damage that happen next.
```

* I will continue to update this EFI _periodically_ as long as im using it. This repo will be archived if im no longer using this OS.

### **Note:** You need to generate your own SMBIOS to signin an Apple ID
Use CorpNewt's [GENSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate platforminfo using **MacBook10,1** as an SMBIOS for Ventura. Head to [Dortania's haswell platforminfo guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#platforminfo) for in-depth guide.

## latest changes (31 Aug)
* Initial release based on OpenCore 1.0.1
* Post-Install patch using OpenCore Legacy Patcher 1.5.0

## Step-By-Step Guide
* Build OpenCore Ventura installer or use my EFI provided **(Using "MacBook10,1" SMBIOS)**.
* Download latest OpenCore-Patcher.pkg from [OpenCore-Legacy-Patcher Repository](https://github.com/dortania/OpenCore-Legacy-Patcher) and keep it somewhere safe.
* Boot into installer you may experience slow graphic caused by low gpu vram. (Fix by OCLP)
* Once the installation finish. Install **OpenCore-Patcher.pkg** open OpenCore-Patcher app select Post-Install Root Patch and click Start Root Patching.
* Restart and it should be working fine

### Known issues (Update 31 Aug)
* Most issues come from OpenCore itself see [OpenCore Lenovo Z50-70](https://github.com/JuicerV3/Opencore-Monterey-Z50-70).
* Unable to grant special permissions to apps (ie. Camera Access to Zoom, Discord Microphone) [Workaround click here](https://dortania.github.io/OpenCore-Legacy-Patcher/ACCEL.html#unable-to-grant-special-permissions-to-apps-ie-camera-access-to-zoom)
* [Legacy Metal Graphics issues](https://github.com/dortania/OpenCore-Legacy-Patcher/issues/1008)

### What works (Update 31 Aug)
* WiFi & Bluetooth
* Ethernet
* Onboard Audio & Microphone
* Display Brightness Control
* Webcam
* USB 2.0 & 3.0
* Battery read-out (Battery percentage)
* Keyboard & Trackpad
* Volume keys
* Sleep & Wake (Need more testing to confirm)

More info on my [OpenCore Lenovo Z50-70](https://github.com/JuicerV3/Opencore-Monterey-Z50-70) Repository

## Links/Guides
* https://github.com/dortania/OpenCore-Legacy-Patcher (OCLP)
* https://openintelwireless.github.io/itlwm/ (Native Intel WiFi)
* https://openintelwireless.github.io/IntelBluetoothFirmware/ (Native Intel Bluetooth)
