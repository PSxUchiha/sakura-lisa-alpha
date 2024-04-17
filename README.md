## Project Sakura Alpha build for Xiaomi 11 Lite NE 5G(lisa)

This is an unofficial user build for testing purposes, in order to flash yourself follow the following steps:

1. First, reboot your device into fastboot mode by holding down the appropriate button combination (Volume Down + Power) until the word FASTBOOT appears on the screen.
2. Open an ADB & Fastboot tools window on your PC and flash the LineageOS Recovery images you downloaded before.
3. 
   ```
   # cd to the directory where your .img files are located before running these

   fastboot flash boot boot.img
   fastboot flash vendor_boot vendor_boot.img
   fastboot flash dtbo dtbo.img
   ```
4. Reboot your device into recovery mode by holding the appropriate button combination (Volume Up + Power) until LineageOS Recovery shows up on the screen.
5. On the screen, tap Factory reset, then Format data/factory reset and press Format data. This will delete all your device's data and remove encryption from an older ROM.
6. ```
    # On the device, Tap `Apply update`, then `Apply from ADB` for starting the sideload service
    # On the computer, sideload the package using this command (Mention the path of the Sakura zip before running the command):
    adb sideload <path/to/Sakura/rom>.zip
   ```
