# Backing up Important Partitions

This guide will show you how to back up important partitions which are unique to each device.

It is extremely recommended to backup these partitions which contain your IMEI/broken celluler or modem network etc. If your device bricks or if those partitions get corrupted, without having backups you will
not be able to restore your IMEI or celluler networks at all!

Table of Contents:

* [Backing up Important Partitions)](#backing-up-Important-Partitions)
   * [Files/Tools Needed](#filestools-needed)
* [Steps](#steps)
   * [Booting to TWRP](#booting-to-twrp)
   * [Backing up partitions](#backing-up-partitions)

## Files/Tools Needed

- A Galaxy A52 4G
- UEFI and TWRP images
- SDK platform tools
- A Windows PC to work with the device

## Disclaimers

> [!WARNING]
> - Run commands exactly what is shown here for a5q. dont run your own commands. misuse of dd tool can lead you destroy your phone!!

# Steps

## Booting to TWRP

If you don't currently have TWRP flashed on your device, please follow the [Flashing TWRP and UEFI on Galaxy A52 4G](Flash-UEFI-TWRP.md) guide first.

You can boot to TWRP recovery by doing these steps:

- Power off the device
- Connect your device to the PC with a USB cable
- Hold Power + Volume up buttons



## Backing up partitions

- Open a Terminal / Command prompt on your Windows computer (make sure that ADB executable is on PATH)

- Enter the TWRP shell

```bash
adb shell
```

- Run these commands to back up the partitions

```bash
mkdir backup

dd if=/dev/block/by-name/efs of=/backup/efs.img
dd if=/dev/block/by-name/fsc of=/backup/fsc.img
dd if=/dev/block/by-name/modem of=/backup/modem.img
dd if=/dev/block/by-name/modemst1 of=/backup/modemst1.img
dd if=/dev/block/by-name/modemst2 of=/backup/modemst2.img
dd if=/dev/block/by-name/sec_efs of=/backup/sec_efs.img
dd if=/dev/block/by-name/fsg of=/backup/fsg.img

exit
```

- Now use the adb pull command to fetch the backed up partitions to your computer

```bash
adb pull /backup .
```

The above command will fetch all the backed up partitions from your device to the current directory on your PC.
we're done, please keep the backed up partitions in a safe place on your computer.
