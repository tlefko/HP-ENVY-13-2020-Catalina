# HP ENVY 13 2020-Catalina (10th Gen Tested)

# News
In light of the recent WWDC, we will begin testing the functionality of our EFI on macOS 11 for this device with the latest developer preview
Version Info

# Features and Overview
- Now Compatible with 10.15.6
- Please leave feedback with issues or w/o
- Comitted to Updating up to OS 11
- Multitouch Trackpad Support
- 4K @60 Hz
- Fixed Bluetooth and Wifi Stability Issues
- Preformance and Power Management
- Additional Patches for 4K Display
- updated for 15.6 rev 1
- Sleep Wake is functional for some models ----if screen glitches on wake or reopen lid. If this is a bother just disable sleep. This is issue is resolved in Big Sur

# Bugs
- Some models may experience screen split in half. If so disable.
- USB devices eject (external)
- No Internal Mic

# What Works
- Everything minus sleep issue above, internal microphone. (audio is fine, headphones / usb mic fine, just not laptop mic)

# POST
run sudo pmset -a hibernatemode 0

# Description
This esentially an ultra-simplistic version that is stable without the use of a deploy or complicated file installations and copies.
You can easily view all the DSDT patches along with configuration files for the bootloader as they are all documented clearly in the files.
This does include a copy of Clover, which of course I do not contribute to and am only responsible for the provided files, patches, and kext placements
This guide provides a working setup with little knowledge of the topic and without "optimization" (because often they can break things). But, it is fully functional and preforms properly and is stable.

# Unsupported Wifi
- Make sure you are using DW1560 or 1820a for wifi or else there is a risk of KP. If not using remove BRCM kexts from CLOVER>kexts>other

# Styling
This guide is designed to be literally as thorough as possible to appeal all types of users. It does not cover complex topics like undervolting etc etc only to provide a completely functional system

# Notes
- Never tested USB C except for charging, USB, works great (not sure about DispOut)
 - 4K model has  sleep wake issues occasionally, 1080P is fully functional
 
 # BIOS
 - Disable Secure Boot
 - Disable Vt-d
 
 # Recommended: Clean Install (Preinstall steps)
- Format a USB (16GB) as Journaled and then proceed to download the latest Catalina Installer Patcher Application.
- Download the latest Catalina installer from within the Patcher App, and select to download a new copy and install to your USB device
- Download the clover configurator application and mount the EFI of the USB partition, then copy the contents of the Files linked above to A new EFI Folder (that you create) within the EFI partition.

** This is because the App Store installers will often not download a full installer, just an truncated version that downloads the installer files from the interent while installing. Thus, they're not bootable from a USB as they're not complete. That is why you should use this method to make sure the installer is usable for bootable media.

# Boot From USB
- Use f9, copy EFI folder to efi partition of your usb. after installation complete copy EFI to your ssd.

# Boot Entry Setup
- Reccomend using windows to find a tool to add a UEFI bios entry to boot EFI/Boot/bootx64

# Credits
- @MaLd0n for DSDT Patches and support (HUGE SHOUTOUT)
- Original Kexts Authors
- Clover

# Headphones and Audio
- All audio from speakers should work perfectly along with Bluetooth and USB audio

# Finished!
Congratulations, there really aren't any more steps that are required. Feel free to contact me with any questions.

# Donations
Send me a coffee lefkotyler@gmail.com


