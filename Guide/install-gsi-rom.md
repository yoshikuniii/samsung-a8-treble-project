# GSI ROMs Guide

I assumed that you have followed insctruction and successfully [install custom recovery]() and [treble our device](). Now, we can install GSI ROM!

Here links to collection of GSI ROMs : [https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list](https://github.com/phhusson/treble_experimentations/wiki/Generic-System-Image-%28GSI%29-list)

Before you download the GSI ROM, please follow this instruction :
- Our device can use **GSI that came with Android version 9, 10, and 11** (depends on vendor installed).
-> Some people manage to install GSI with Android 12, but buggy.
- Our device **use VNDKLite**, so download ROM that use VNDKLite.
- Our device support **A/B Partition**.
- Our device is **ARM64 architecture**.

So, in summarize you need download the image named:
**system-arm64_[xyZ]-vndklite.img**

- **x** can either be **a** or **b**
- **y** can either be **v**, **o**, **g** or **f**
- **Z** can be **N** or **S**

**b** = a/b --> **we must download this variant.**
**a** = a-only  
  
**g** = gapps  
**o** = gapps-go  
**v** = vanilla (no gapps included)  
**f** = floss (free & open source apps instead gapps)

**N** = no superuser  
**S** = superuser included  
**Z** = dynamic superuser included

**-lite/vndklite** = for VNDK Lite vendors (also can help with broken camera even on normal VNDK vendors).

Example : **arm64-BvZ-vndklite.img** is ARM64 with A/B partition, vanilla, with dynamic superuser included, and use vndklite.

***
# Installing ROM
Let's say you found your GSI ROM, and you have downloaded the file. If file you download comes with *.xz* format, you need to extract it.

To install ROM:
1. Boot to recovery, then **copy/move extracted image** to your phone .
2. Flash image from recovery and **flash as system image**.
3. Back to TWRP homescreen, touch **Reboot > Recovery**. 
4. Then, **Reboot > System**. 

# List of Usable ROM
This list are ROM that I've installed on my Samsung A8, some stable, some have bug on it, and some cannot be installed. For this, I use vendor Quack v2.6.

- Vendor from Android 10, can install ROM Android 11 (**Contain bugs like third-party camera app crashing, VoLTE and Bluetooth calls**.).
- You can install **Android 12 GSI, but don't use lock screen** (pin, password, fingerprint, face unlock), it will cause bootloop and can't boot to TWRP. You need to flash stock ROM. 
- Android 12 have a lot bugs.
- Whats work and not, check [this](https://github.com/phhusson/treble_experimentations/wiki/Samsung-Galaxy-A8-(Exynos)) for more info.

| Android Version | ROM Name | Review | Thread/Download |
|--|--|--|--|
| 11 | CAOS | Stable enough, lack of customization, need no reboot after a couple days. | [Thread](https://forum.xda-developers.com/t/official-aosp-r-mod-caos11.4265059/) |
| 11 | Corvus OS | Can't install, bootloop. | [Thread](https://forum.xda-developers.com/t/gsi-alpha-11-phh-corvus-v12-5-xmas.4212765/) |
| 11 | Dot OS | Bugs on camera and torch, other seems stable. Good looking OS, a lot of customization. | [Download](https://www.droidontime.com/devices/arm64) |
| 11 | Ancient OS | Stable, a lot of customization | [Download](https://sourceforge.net/projects/ancientrom/files/gsi/) |
| 11 | Lineage OS 18.1 | Stable, lack of customization | [Thread](https://forum.xda-developers.com/t/gsi-11-lineageos-18-x-gsi-all-archs.4205461/) |
| 11 | OneUI 3.1 M31 Port | Stable enough, some feature have bugs like: can't use Samsung Camera (3rd party camera works), Jack has some faint noises while no media is playing, face unlock and torch intensity control. **This is most stable ROM I ever use.**| [Thread](https://forum.xda-developers.com/t/rom-vendor-oneui3-1-m31-port-treeui-0-9-4-beta-for-a8-a8-a7.4239353/) |
| 11 | OneUI 3.1 S20 Port | Same like M31 Port, feature on VoLTE (experimental option available, some Indians had luck with that, and DBT CSC | [Thread](https://forum.xda-developers.com/t/rom-vendor-oneui3-1-s20-port-treeui-0-9-5-beta-for-a8-a8-a7-m20-m30.4252235/)
| 10 | Havoc | Stable, a lot of customization | [Download](https://sourceforge.net/projects/havoc-os/files/) |
| 10 | CAOS | Stable, decent customization | [Thread](https://forum.xda-developers.com/t/official-aosp-q-mod-caos.4137289/) |
| 10 | /e/ OS | Stable, deGoogled ROM that respect your privacy. Actively maintened by developer, it has updated security patch, so this is currently the best ROM you can install.| [Link download and how to install the ROM](https://doc.e.foundation/support-topics/install-GSI) |

