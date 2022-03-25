<h1 align="center">Google Camera Module</h1>
<h3 align="center">for kenzo/kate devices</h3>

This module fixes some issues currently encountered on Redmi Note 3 and Redmi Note 3 Pro when using modified Google Camera by replacing original cam libraries with modified one's.
It also enables some features not present in custom ROMs.

This module is to be used at your own risk, this is a fork of Abhishek's module, I updated the module to work with Android 11.

## Working
Currently this module virtually adds/replaces libs/files in `system/vendor/lib` `system/vendor/etc`,  modules can be deactivated through magisk to revert back to the stock functionality..

## Compatibility
- This module is compatible with Android 11.
- for previous version of Android use v1.4 for better functionality. 
## Current List of Features
1. Enables 60 FPS video recording
2. Fixes green tint on front camera
3. 4k DCI Support
4. Increased Maximum ISO value - 12,800
5. Constant framerates when shooting videos
6. Improved Denoising for 30 fps videos


## Who did what ?
- [**SerJo87**](https://forum.xda-developers.com/member.php?u=5074663) and [**Kiraryu**](https://forum.xda-developers.com/member.php?u=8549930) modified the the initial libs that enable 60fps recording. (Currently not using the libs)
- [**Savitar(defcomg)**](https://forum.xda-developers.com/member.php?u=377973) edited the libs to increase maximum ISO and improve denoising.
- [**Kuro Shi**](https://t.me/Kuro_Shi_Sama) modified the libs that fix green tint.
- [**Ayush**](https://t.me/AyushR1) modified libs for lag fix. (Currently not using the libs)(Not working on A10)
- [**Amogha**](https://t.me/amog787) modified FP keylayout files for goodix/fpc. (Currently not using the files)
- [**Krittin**](https://forum.xda-developers.com/member.php?u=5022949) provided 4k DCI support and additional info about libs, much thanks buddy.
- [**Abhishek**](https://t.me/BoogeyWoogey69) created the magisk module.

**Huge thanks to everyone who helped to make this module possible !**

## Special Thanks
- [***topjohnwu***](https://github.com/topjohnwu) for [magisk](https://github.com/topjohnwu/Magisk) and official [template](https://github.com/topjohnwu/magisk-module-installer).
- [***Zackptg5***](https://github.com/Zackptg5) for [MMT-Extended](https://github.com/Zackptg5/MMT-Extended) template.

## Support
- Telegram Channel - https://t.me/modified_gcam_rn3
- Telegram Group - https://t.me/rn3photography

## Changelogs
### 1.5-A11
- Support for Android 11, for previous version of Android use v1.4 for better functionality.
- Removed libs causing non boot. 
- removed swcodec (not needed?)
- Based off Abhishek's module.

### 1.4
- Support for Android 10.
- Upgraded to MMT-Extended (MMT-Ex) template from Unity (frequently updated by Zack).
- Fixed device booting into fastboot mode as some libs were'nt compatible with Android 10.
- Updated media profiles to be compatible with Android 10.
- Added Codec2 support libraries/files and enabled them in `system.prop`.

### 1.3
- Upgraded to Unity Template v4.4 (more features/options over stock).
- Enabled Minimum API detection above API Level 26 (8.0.0 - Oreo). Below this API Level, no android versions are supported.
- Install Script cleanup
- Removed Fingerprint Shutter as requested by most users (Maybe i can make it optional in next update).

### 1.2
- Added 4k DCI support
- Increased max ISO from 6400 to 12800
- 60 fps video recording now working in 6.3
- Improved Denoising
- Framerates are now constant when shooting videos
- Changes to media_profiles.xml

### 1.1
- Reverted primary camera vendor blobs back to stock MIUI. This enables stock video recording on snapcam and also works with GCam 6.X (Currently Tested).
- Added device check for kenzo and kate.
- Changes to media_profiles.xml

### 1.0
- Initial Release