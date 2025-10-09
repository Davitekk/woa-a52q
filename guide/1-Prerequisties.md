# Install Windows on Galaxy A52 4G
Before you begin installing windows on your A52, make sure you have the following things

## Prerequisties:
   - PC / Laptop with Windows (Recommended: Windows 10 or higher/ Any Linux distro like Ubuntu 24.0 or latest )
   - [ADB](https://developer.android.com/studio/releases/platform-tools#downloads)
   - [TWRP](https://twrp.me/samsung/samsunggalaxya52q.html)
   - Unlocked Bootloader ( [Unlock the Bootloader](../UnlockingBootloader.md) from here)
   - [UEFI Image](https://cdn.discordapp.com/attachments/1214286539593613344/1425171690089877635/Mu-a52q.img?ex=68e89851&is=68e746d1&hm=f10b087c98648d498cd1e3b4edab407c4190704de889639ae48902470d309151&)
   - install.wim from a Windows 11 24H2 ISO
   - [Parted](https://cdn.discordapp.com/attachments/1057409313381040261/1275435724195496048/parted?ex=68e85755&is=68e705d5&hm=5ac60912de2fbd785f2e83c9ecf1d613a49b486141d215013d2d0382f9685a6c&)
   - [GDisk](https://cdn.discordapp.com/attachments/1057409313381040261/1319684671486824478/gdisk?ex=68e87a60&is=68e728e0&hm=0a4e2dad4c8e716b8dcf06387149b984cbdb6bbec7bc2859fe939bc6e58a8de6&)
   - [A52q drivers](https://github.com/woa-a52s/Samsung-A52s-5G-Releases/releases/latest)

Table of Contents:
   * [Files/Tools Needed](Prerequisties)
* [Steps](#steps)
   * [Unlocking the Bootloader](#unlocking-the-bootloader)
   * [Flashing UEFI and TWRP](#flashing-uefi-and-twrp)
   * [Backing up Important Partitions](#backing-up-important-partitions)
   * [Fixing UFS GPTs and its LUNs](#Fixing-UFS-GPTs)
   * [Partitioning](#partitioning)
   * [Activating Mass Storage Mode](#activating-mass-storage-mode)
   * [Installing Windows](#installing-windows)
   * [Installing the drivers](#installing-the-drivers)
   * [Boot Windows](#boot-windows)

## Step-1
## Unlocking the Bootloader

If not already done, please first proceed with the [Unlocking the Bootloader](../UnlockingBootloader.md)) guide for Galaxy A52 4G. Come back once you're done. If you already followed this guide, please skip the unlocking section.

## Step-2
## Flashing UEFI and TWRP

If not already done, please first proceed with the [Flashing TWRP and UEFI](../Flash-UEFI-TWRP.md) guide for Galaxy A52 4G. Come back once you're done.

## Step-3
## Backing up Important Partitions

It is highly EXTREMELYT recommended to [backup important partitions](../BackingUpImportantPartitions.md) that are unique to each device before proceeding with the guide.

Please follow the provided guide, then come back once you're done.

