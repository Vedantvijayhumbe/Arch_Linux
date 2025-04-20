# Arch_Linux
Arch Linux setup guide with common errors and debugging methods . 
<img src="https://github.com/user-attachments/assets/66dca052-8138-48ba-9b18-d76025b40720" alt="drawing" width="200"/>

**Why Arch Linux**
 - "The Arch Way" + By far the biggest and most up-to-date software collection with the official repos + AUR.
   That's what makes Arch great.
   https://www.reddit.com/r/archlinux/comments/34qujf/why_arch/


**STEPS** :

1. Go to this website :  https://archlinux.org/download/ . Then navigate down to your country and see for the latest versions of arch available over there .
2. Download (it happens just by click ) both .iso and .sig (as it is later necessary for verification ) .
3.  Verify signature
    It's recommended to verify the image signature to ensure you're not installing a tampered ISO.
    to do this at the start(I advice you to do so)  , on cmd (run as administrator) :
    download gpg from https://gpg4win.org/  (During install, keep "Kleopatra" selected (it’s the GUI for GPG)) . then : 
   ```
    gpg --keyserver-options auto-key-retrieve --verify archlinux-version-x86_64.iso.sig
```
   if you are doing this in the later stages then do this from an existing Arch Linux installation :
   ```
pacman-key -v archlinux-version-x86_64.iso.sig
```
4. You'll see the .iso and sig being installed in downloads on your windows downloads directory . but that is not your real setup . you need to move this to a portable device such USB . to write it to the USB use tools such as **Rufus** .
download link : https://rufus.ie/en/

keep other stuff intact . 
5.what if I wanna keep both windows and arch linux is this possible? 

Yes, it's absolutely possible to dual-boot Windows and Arch Linux on the same device! You'll set up a system where both Windows and Arch Linux coexist, and you can choose which one to boot into when you start your computer.

to do this you need to shrink your windows partition first , so that memory can be allocated to the arch .

to do this use MiniTool Partition Wizard Free 12.9. link : https://www.partitionwizard.com/free-partition-manager.html 
6. make sure USB frive where we shifted our downloaded arch is connected to your PC , now reboot using Fn+F12 . 

https://www.youtube.com/watch?v=LWhoQnWH4Co
   
