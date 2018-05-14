# Mediacom Phonepad Duo G5M rooting guide


This simple guide help you to gain root access in this terminal with MTK6580 and Android 7.0 Nougat.

**Attention: the rooting procedure invalidates the warranty or could brick your device, executing the guide you assume your responsibility is your choice.**

**Read before start:** For gain root permission you will need to unlock bootloader, this erase all your data. You must do a backup if you can't lose them. If you have already unlocked the bootloader you can skip to step 3

1) Enable dev opts
2) Unlock Bootloader
3) Install Magisk 
4) Go Happy (if you don't brick your phone)

Magisk is a open-source project used for gain root, hide root to app, install modules, etc. For more info check this link:

Magisk xda page [here](https://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445)

**1) First step is enable Dev Options for unlocking bootloader:**

>  1) Go into Settings
>  
>  2) Scroll to the bottom and select About phone.
>  
>  3) Scroll to the bottom and tap Build number 7 times.
>  
>  4) Go back and enter into new menu item - "Developer Options"
>  
>  5) Scroll down until OEM unlocking and enable it
>
>  6) Then enable USB debugging too
  
**2) Second step is unlock bootloader**

>  1) Open terminal and digit
```
  adb reboot bootloader
```
>  2) When the smartphone is in fastboot mode, digit
```
  fastboot oem unlock
```
>  3) If the unlock was a good end you can see into OKAY into terminal, the you can reboot the smartphone with command
```
  fastboot reboot 
 ```
 
**3) Third step is for install Magisk

>  1) Go into Security, scroll down until "Unknown sources" and enable it
  
  
>  2) Copy Magisk apk into your device **or** run
 ```
  adb install /path/to/locate/MagiskManager-v5.7.0.apk
 ```
 
**4) Fourth step is for flashing patched_boot.img

>  1) Open terminal and digit
```
  adb reboot bootloader
```
>  2) When the smartphone is in fastboot mode, digit
```
  fastboot flash boot /path/to/locate/patched_boot.img
```
>  3) Wait, if flash was a good end you can see OKAY in terminal, then you can reboot with command
```
  fastboot reboot 
 ```
 
 **5) Fifth step only for check if you have root permission
 
 >  1) You can download anyone app for root check (like root checker) and you can see if you are now root
 
 >  2) Enjoy
