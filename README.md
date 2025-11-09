# Root-vivo
This is one of the method to root vivo phones after bootloader is unlocked
## Warning i am not responible for Bricked devices and unusable devices

## prerequisites
### ADB
To set up adb watch this video 
https://youtu.be/26GI3z6tI3E?si=CyTh9nLRGutm_M6u
### Official frimware from vivo
Get the latest frimware from https://www.vivo.com/in/support/upgradePackageHome
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
* Step 1: Get the latest frimware from https://www.vivo.com/in/support/upgradePackageHome
* Step 2: Unzip the file and sent the boot.img and vbmeta.img file it to your vivo device (you can use adb or just use the filemanager on the system(pc)
### Step 3 : Patch boot.img file 
* Step 1: sent the boot.img and vbmeta.img files(from the zip file you just unzipped) to your vivo device (you can use adb or just use the filemanager on the system(pc)
* Step 2: Download magisk from https://github.com/4accccc/vivo-Magisk-suu because the original magisk is blocked by the kernal of vivo
* Step 3: open the app and select the boot.img file 
* Step 4: Get the new patched file from the device (you can use adb or just use the filemanager on the system(pc))
* Step 5: Open terminal(cmd,power shell, kitty,etc) and run ```adb reboot bootloader``` and run ```fastboot flash boot magisk_patched.img``` replace magisk_patched.img to your magisk patched image and run ```fastboot reboot```
* The device is now rooted

### Check whether the wifi and bluetooth works or not.
if it wont work .The reson is due to the boot.img file you patched has compactablity issues 
find the software version of the preinstalled software it somewhat looks like this PD1987F_EX_A_6.70.72
compare them with the zipfile you downloaded in my case the latest vertion given by vivo on their site is PD1987F_EX_A_6.70.72 and the pre installed frimware is this PD1987F_EX_A_6.71.42 which is greater than the official site has given
that caused the problem 
#### If the installed version is less than the official version 
* Step 1: Move the zip file (offical frimware from vivo) to your phone (you can use adb or just use the filemanager on the system(pc) and open terminal and type ```adb reboot recovery```
* Step 2: Select install software and click local install click the zip file you just moved to your phone
* Step 3: do all the step from ``` In Rooting vivo phones ```
* Done
#### If the installed version is Greater than the official version 
  
