# Mediacom Phonepad Duo G5M rooting guide


This guide help you to gain root access in this terminal with MTK6580.

**Attention: the rooting procedure invalidates the warranty or could brick your device, executing the guide you assume your responsibility is your choice.**

**Read before start:** For gain root permission you will need to unlock bootloader, this erase all your data. You must do a backup if you can't lose them. If you have already unlocked the bootloader you can skip to step 3

1) Enable dev opts
2) Unlock Bootloader
3) Install Magisk 
4) Go Happy (if you don't brick your phone)

Magisk is a open-source project used for gain root, hide root to app, install modules, etc. For more info check this link
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
  
