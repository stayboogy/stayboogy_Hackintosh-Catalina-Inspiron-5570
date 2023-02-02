# stayboogy_Hackintosh-Catalina-Inspiron-5570

- I have a real Macbook which is what makes most of this possible, just fyi.
- starting from scratch without one isn't impossible but not as simple, nor allows clean access to the Catalina installer

# stayboogy_Hackintosh-Catalina-Inspiron-5570

- Everything needed to Install and Boot Catalina on the Dell Inspiron 5570

## Installer 

- https://www.mediafire.com/file/ie11wulj3x5u0ps/Catalina_stayboogy.img/file

## My Device:

- Dell Inspiron 5570 with i5-8250U with 1920x1080 full HD display and 12GB of RAM (upgraded) and 1TB SSD (upgraded).

- Must have Sata Mode set to AHCI in BIOS in order for the installer to see your hard drive (perhaps just for SSDs) and then you can go back to RAID once you are installed and booting, and you should. Nothing else has to be changed despite what others have incorrectly stated.

## What doesn’t work:

- OEM supplied wifi card--bluetooth works
- Waking from sleep on AC power

## What does work:

- Camera
- USB
- OEM bluetooth connection
- Waking From Sleep on battery
- FileVault Encryption with APFS without boot lag
- Ethernet
- HDMI video and audio out
- Audio—speakers, mic, headphones
- Video/Graphics
- Backlight Keyboard
- Trackpad, not quite like a real Mac but real close
- Fn Keys—Volume + -, skip, play, pause, forward, back, keyboard backlight, Display backlight dim and brighten, etc
- CPU Management and Thermal Control (as far as I can tell, as the fan cuts on properly and adjust speeds as necessary)
- SSD compatibility with no lag
- with proper SMBIOS information editing in config.plist (easy to find here on GitHub), FaceTime, iMessage, iCloud, etc, all working perfectly


- I am very satisfied with this and how it runs on my laptop.  It works damn near to perfection especially with a proper m2 wifi card.

- SIP is disabled by default and unverified kexts are allowed and mounting of root filesystem as rw is possible and gatekeeper can be disabled.