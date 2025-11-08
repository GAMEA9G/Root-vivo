# Root-vivo
This is one of the method to root vivo phones after bootloader is unlocked
## Warning i am not responible for Bricked devices and unusable devices
## Rooting
Rooting in simple words is just patching the boot.img file to gain super user access
generally rooting steps are
* Step 1: Unlock bootloader(assume you have done this)
* Step 2: Get the boot.img file
* Step 3: Patch it and flash it
* Done
## In Rooting Vivo phones
Assuming you have done the step one
### Step 2 : Get The boot.img File
* Step 1: Get the latest frimware from https://www.vivo.com/in/support/upgradePackageHome and compare them with pre installed software (stock)
* Step 2: Unzip the file and sent the boot.img and vbmeta.img file it to your vivo device (you can use adb or just use the filemanager on the system(pc))
* Step 3: Download magisk from https://github.com/4accccc/vivo-Magisk-suu because the original magisk is blocked by the kernal of vivo
* Step 4: open the app and select the boot.img file 
* Step 5: Get the new patched file from the device (you can use adb or just use the filemanager on the system(pc))
* Step 6: Open terminal(cmd,power shell, kitty,etc) and run ```adb reboot bootloader``` and run ```fastboot flash boot magisk_patched.img``` replace magisk_patched.img to your magisk patched image and run ```fastboot reboot```
* The device is now rooted check whether the wifi connects or not. if not do this (
  * 
