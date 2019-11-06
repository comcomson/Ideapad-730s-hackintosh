# Ideapad-730s-hackintosh
This Clover config work for Lenovo Ideapad 730s
# Credits
# What is NOT WORKING
* WiFi + Bluetooth
* Fingerprint (disabled)
# What is WORKING
* PS2 Keyboard  [VoodooPS2Controller.kext](https://github.com/alexandred/VoodooI2C/releases/latest)
* TouchPad work with SSDT fix, [VoodooI2C.kext](https://github.com/alexandred/VoodooI2C/releases/latest). 
* Battery and cpu sensor, [VirtualSMC.kext](https://github.com/acidanthera/VirtualSMC/releases/latest). 
* USB [USBInjectAll.kext](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads)
* SSD Trim by Clover patch 
* Camera works fine
* Hibernation and wake up
## BIOS setting before install
* Disable Security -> Intel SGX -> Intel SGX Controller
* Disable Security -> Secure Boot
* Switch RAID to AHCI in Configuration -> SATA Controller Mode

## FAQ

- Q: Touchpad not work on First boot?  
  A: Enter command `sudo kextcache -system-prelinked-kernel` in terminal and reboot
- Q: Can't boot Win10 when BIOS swtch to AHCI?  
  A: Boot Win10 in [Safe Mode](https://support.microsoft.com/help/12376) 
