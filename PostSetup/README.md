- DO NOT REBOOT after MacOS loads--open the clover app from the PostSetup in this repo which you should have copied to another usb.  

- Mount your EFI partition of your laptop with Clover.  Open the EFI in Finder and delete the EFI folder completely, and then copy the PostSetup EFI folder from this repo to the EFI partition.

- Remove the usb and reboot.

- If your laptop does not boot directly into Clover Bootloader, use F12 and boot into the BIOS and add /EFI/CLOVER/CLOVERX64.EFI of your hdd as the boot path to your UEFI boot options menu.

## You should now have MacOS Catalina running on your 5570 like it was built for it.
