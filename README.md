# Msi-Gf63-10scsr-Sonoma-Hackintosh-EFI
This Repository Has A EFI That Uses Opencore 1.0 And Supports Sonoma, The Latest And Greatest For MSI gf63 10scsr

[![OpenCore](https://img.shields.io/badge/OpenCore-1.0.-blue.svg)](https://github.com/acidanthera/OpenCorePkg)
[![macOSver](https://img.shields.io/badge/macOS-12.6.1-brightgreen.svg)](https://support.apple.com/HT213494)

![51Rf3zw4rIL _AC_SL1000___1_-removebg-preview](https://github.com/Envadors/Msi-Gf63-10scsr-Sonoma-Hackintosh-EFI/assets/91122426/c464e44d-02e7-4c8d-baf0-890be9126e7c)

------------------------------------------------------------------------------------------------------

- [EFI For macOS Sonoma](https://mega.nz/file/GugEgKIB#5-PMXh4OGy75J0TyXq-9s69kDM5lMJs8uryR_nJFRJc)
- [EFI Link For macOS Ventura Until Big Sur](https://github.com/Forte500/Hackintosh-msi-GF65-10UE)


------------------------------------------------------------------------------------------------------

### ✅️ What works</strong></summary>

- iGPU acceleration Intel UHD 630 2048 MB
- Sleep
- Power management
- Audio (speaker, microfone, headphone jack)
- Battery percentage
- USB ports
- Display Brightness
- Wifi & Bluetooth
- iMessage
- Dual Boot with windows 10 & 11
- Keyboard
- Brightness & volume FN keys
- Trackpad
- Internal camera
- Ethernet port
- Continuity: Handoff & Universal clipboard
- AirPlay: `iPad -> Mac` & `Mac -> TV`
- Sidecar wired
- *Sidecar wireless with broadcom card only

### ❌️ What doesn't work
- Video output over USB-C
- Apple Watch Unlock, Universal Control, Instant Hotspot with broadcom card
- HDMI Since The Port Is Wired To NVIDIA.
- NVIDIA Graphics Card As MacOS Never Nativity Supported It.
- Backlight But Who Ever Uses It Am I Right?!

### ⚠️ Known issues
- Wireless sidecar may lag (tested with BCM94360NG & iPad 6 ios 15.1)

⚠️ If Your Not Going To Use Icloud For Your Computer Which I Highly Suggest You Dont Use Icloud, because that results into you just putting the efi on the usb and adding the installer instead of spending 5 hours chainging the serial number. ⚠️

### 💻 My Hardware
| Component       |  Brand/info                                                             |
|-----------------|-------------------------------------------------------------------------|                                   
| CPU	             | Intel Core i7 10th Gen (also compatible with Intel Core i5 10th Gen)   |
| Graphics Card	   | NVIDIA GTX 1650 TI with Max Q Design (disabled on MacOS)               |
| RAM	             | 16GB                                                                   |
| Storage	         | 1.5TB                                                                  |
| WiFi Card        | Intel Wi-Fi 6 AX201                                                    |
| Bluetooth	       | Integrated with Wi-Fi card                                             |
| Laptop Keyboard	 | VoodooPS2                                                              |
| Touchpad	        | VoodooPS2                                                              |

❤️ Credits To My Guy On Reddit Named Forte500 For Providing Me With The EFI That Works For Ventura And Monetery And BigSur.
Credits To Me On Updating The EFI To Opencore 1.0 And Making It Support Sonoma, I Have Eliminated As Much Bugs As Possible.
Thank You And Enjoy Your Hackintosh EFI, I Hope Everything Goes Well! ❤️



## 🛠 UEFI - Bios Settings
<details>
<summary><strong>UEFI Custom Hackintosh Settingse</strong></summary>
  <br>
 
- Show hidden settings with: CTRL Right + SHIFT Right + ALT Left + F2 
- Turn off Secure Boot [Security] 
- Turn off CFG Lock [Advanced -> Power & Performance -> CPU -> CPU Lock Configuration]
- Disable Fast Boot [Boot]
- Select UEFI mode without CSM [Boot]

</details>

## 🛠 Post-install
<details>
<summary><strong>Copy EFI to the internal drive</strong></summary>
  <br>

1. Open terminal. Type `sudo diskutil mountdisk disk0s1` (disk0s1 corresponds to the EFI partition of the internal disk)
2. Open Finder and copy the entire EFI folder from your USB to the root disk's EFI partition.
3. Unplug the USB device and reboot your laptop, while rebooting hold down `F10 Or F11` to access the boot menu.
4. Boot from `Kingstone-579420` (or your ssd's name).
5. To check that everything has gone well repeat `step 3` and look for a new entry called `OpenCore`
4. Now you can boot macOS without your USB device. ✅️

</details>

## 🛠 SMBIOS
<details>
<summary><strong>Make A Serial Number To Get Icloud Running</strong></summary>
  <br>
  
1. Prepare your config.plist which you've made.
2. Download or clone the whole repo of [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS).
3. Open the folder and open GenSMBIOS.bat \(on Windows\) or right-click open GenSMBIOS.command \(on macOS\)
4. Enter 1 and enter. \(for update/install MacSerial\)
5. Then enter 2 and enter.
6. Drag and drop your config.plist and press enter.
7. Y.
8. Enter 3 and enter.
9. Enter the SMBIOS you want to generate and enter the number of SMBIOS amount. Press enter. **For AMD System,** here is the list of SMBIOS recommended from the most to the least: - _**iMacPro1,1**_ \(most recommended\) - _**iMac14,2**_ ****\(also recommended\) - MacPro6,1 \(a little bit old but it works\) - MacPro5,1 \(outdated and already lost support on Catalina\) - Other SMBIOS \(not recommended as they might cause problems\)
10. The first SMBIOS will be flushed into your chosen config.plist.
11. Icloud Services Should Work Now And Enjoy Your Hackintosh 👍.

</details>

## 🎁 Extras, (Optional)
<details>
<summary>Userful Apps</strong></summary>
  <br>
  
- [Arc](arc.net) * The Best Browser
- [OC Updater](https://github.com/mswgen/oc-updater/releases/tag/1.4.3) * A Opencore Updater That Can Update Your EFI With Just One Click If New Updates Are Found.
  
  </details>
