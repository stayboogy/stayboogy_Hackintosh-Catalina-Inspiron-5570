- I have a real Macbook which is what makes most of this possible, just fyi.
- starting from scratch without one isn't impossible but not as simple, nor allows clean access to the Catalina installer

# Installer_Dell-Inspiron-5570_Catalina

- USB installer image for MacOS Catalina for a Dell Inspiron 5570

## Video Tutorial

- https://youtu.be/6Cb-_b1Hahw

## Before you Install

- Make sure you copy the PostSetup EFI folder from this repo to another usb for use after install

## Download Installer img in a Single File

https://www.mediafire.com/file/ie11wulj3x5u0ps/Catalina_stayboogy.img/file

## How to Install

For Advanced Users ONLY

- This is done in Windows

- Clean, Initialize as GPT, and Format a USB flash drive greater than 8GB to NTFS/FAT32/Whatever in Windows Disk Management.

- Apply the newly combined Catalina_stayboogy.img to your newly formatted USB flash drive using Win32 Disk Imager.

- Make sure SATA is set to AHCI in BIOS--go back to RAID after install and successful reboots of MacOS.

- Make sure boot configuration in BIOS is set to UEFI

- There is a chance you may have to boot to BIOS with the usb in the slot and add the usb as a uefi boot option in the bios with /EFI/CLOVER/CLOVERX64.EFI as the boot path.  This is under boot configuration.  If you don't know what this is or how to add an boot option to your uefi setup, then don't attempt any of this.

- Boot from this usb and install just like you would any other OS--I suggest that you clean install this and format your entire disk and then re-install Windows after.  It's much easier this way and ensures that the proper EFI from my other repo works properly.

- DO NOT REBOOT after MacOS loads--open the clover app from the PostSetup in this repo which you should have copied to another usb.  

- Mount your EFI partition of your laptop with Clover.  Open the EFI in Finder and delete the EFI folder completely, and then copy the PostSetup EFI folder from this repo to the EFI partition.

- Remove the usb and reboot.

- If your laptop does not boot directly into Clover Bootloader, use F12 and boot into the BIOS and add /EFI/CLOVER/CLOVERX64.EFI of your hdd as the boot path to your UEFI boot options menu.

## You should now have MacOS Catalina running on your 5570 like it was built for it.
