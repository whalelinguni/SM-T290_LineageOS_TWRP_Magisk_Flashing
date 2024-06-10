# WIP!!! Uploading Files Now! 
# !!!

# Samsung Galaxy Tab 8 (GTOWIFI) LineageOS + TWRP + Magisk

## Files
```
|[Directory Root]
│   ADB-FASTBOOT-PlatformTools_+_ExtraShit.7z
│   lineage-20.0-20240605-nightly-gtowifi-signed.zip
│   README.MD
│   SAMSUNG_USB_Driver_for_Mobile_Phones_ver_1.5.65.0.7z
│
├───APKs
│       Magisk-v27-0.zip
│       Magisk-v27.0.apk
│
├───FlashFiles_Fastboot
│       boot-lineage20_magisk_patched-27000_aJTiP.img
│       recovery-twrp-3.6.1_11-0-T290XXU3CUK4-20220327.img
│       system-lineage20.img
│
├───FlashFiles_SingleZip
│       lineage-20.0-20240605-nightly-gtowifi-signed_TWRP-3.6.1-MagiskPatchedBoot.zip
│
├───IMG_-Format-Tools_[IMG_TAR.MD5_.DAT]
│       Create-Tar-For-Kernel.7z
│       SDAT2IMG_IMG2SDAT.7z
│       tar-Tool_by_mkh.mourad.7z
│
├───ODINs
│       Odin3 v3.10.7.7z
│       Odin3_v3.13.1.7z
│
└───TWRPS
        twrp-3.6.1_11-0-T290XXU3CUK4-20220327.img
        twrp-3.6.1_11-0-T290XXU3CUK4-20220327.tar.md5
        twrp-3.7.0_11-0-T290XXU3CVG3-20221120.img
        twrp-3.7.0_11-0-T290XXU3CVG3-20221120.tar.md5
```

# Versions:
system: lineage-20.0-20240605-nightly-gtowifi-signed
recovery: twrp-3.6.1_11-0-T290XXU3CUK4-20220327
boot: Magisk Patched v27 boot.img from system above ^^. 

## Flashing files:
Packaged as tar.md5 for odin
Packaged as .img for fastboot
Single ZIP for flashing with tools


# Flashing Notes:
My bootloader was previously unlocked. I did not write any documentation as to what I did.
Magisk patched boot.img taken from LineageOS-20.0-20240605-nightly-gtowifi-signed
I could not get TWRP twrp-3.7.0_11-0-T290XXU3CVG3-20221120 to work. Would not flash correct. ODIN failed. Fastboot Failed.
Flashed with ODIN 3.13.1

ODIN Multi-File:
BL: boot.img		[lineage20_magisk_patched-27000_aJTiP]
AP: system.img		[system-LineageOS-20.0-20240605-nightly-gtowifi-signed]
AP: recovery.md5	[twrp-3.6.1_11-0-T290XXU3CUK4-20220327]

ODIN Single File:
AP: LineageOS-20.0-20240605-nightly-gtowifi-signed.tar.md5 (except you have to use tar-Tool to make this)

I flashed each seperate only because my first all in one zip had TWRP 3.7.0 which failed flashing and the tablet would not boot. 
Trying to diagnose the problem (at that time I did not know it was a TWRP issue) I flashed the 3.6.1 TWRP on since I did not create 
a single zip for that combo. 
I would recommend just converting the lineage-20.0-20240605-nightly-gtowifi-signed_TWRP-3.6.1-MagiskPatchedBoot.zip file to a 
tar.md5 with 'tar-Tool by mkh.mourad' then flashing that in the AP slot with ODIN 3.13.1

Official LineageOS Flashing: https://wiki.lineageos.org/devices/gtowifi/install/



<img src="https://images.cooltext.com/5700528.png">




