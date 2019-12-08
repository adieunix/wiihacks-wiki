---
title: Wiki -> F.A.Q.
description: A wiki maintained by the r/WiiHacks community.
redirect_from: "/faq.md"
---

----

## Modding

   These questions contain information regarding the modding process and the hardware involved.

### I'm ready! How do I mod my Wii?

  * [wii.guide](https://wii.guide/)

  * This is the current approved guide for modding your Wii.

  * Please read and perform every step. Do not skip steps.

  * Do not delete any folders/files that will be generated during the mod process or after.

  * Keeping a backup of these files is strongly recommended.

  * Good luck and have fun.

### Do I need extra hardware?

  * An SD Card, an SD Card Reader, and some form of USB Storage, if you want to minimize risk, a hard drive that isn't powered by the USB.

    You don't need these for every method, but these are what will make it easier as it is the most typical setup.

### Can I do it without an SD Card and or USB Hard Drive/Memory Stick?

  * You can mod your Wii without an SD card. Eventually you will need some form of storage to store your homebrew applications, and your games, whether they be Wii, GameCube, or emulator roms.

### What size should my SD Card be?

  * Anything from 512mb (yeah, I still have one) to 32gb and above have been known to work just fine. You want to make sure it's large enough to accommodate everything you want to put on it, which you can easily figure out by gathering it all together and prepping it on your computer.

### How about the size of my USB storage?

  * Wii games can range from larger than the size of a single DVD and down. If you're a casual player and only have a few games, 100GB would do just fine. However the larger/newer the drives get, the more incompatibilities you might experience.

### Will this HD/SD/ThumbDrive work?

  * Wii compatibility is sporadic, but ones that outright don't work rarely than most people think. I'd suggest checking the [compatibility lists](https://wiihacks.bloodythorn.com/links#storage-compatibility-lists) and if you plan on buying one, make sure the cost is negligible, or the place has a liberal return policy.

### How do I know the current mod/cios state of my Wii?

  * Currently [SysCheck](http://www.hacksden.com/downloads.php?do=file&id=149) is recommended.

### I've botched the process, but my Wii still seems to work, what do I do?

  * To answer a common question on botched installs; NO you do not have to undo anything. As long as your Wii is still (mostly) functional, find some help, start the modding process over. You (almost) never need to undo what you've already done.

### Can I Un-MOD my Wii? Will formatting it remove the mods?

  * Sure. However first warning; you're looking at a procedure far more complex than what you did to mod your Wii.

  * Formatting the Wii will only remove user data. Removing/deleting the SD Card or USB Device will remove all homebrew and games.

  * If you can; updating the Wii might remove *most* of the modified software. Been wanting to make that jump from 4.1 to 4.3? Now's your chance. Just fair warning, this has the potential to brick your Wii.

  * If you were lucky enough to not be able to use an upgrade, you'll want to download all of the stock IOS and replace them all of the modified ones with originals. Of course you'll still need your homebrew to do this with... The suggested tool would be the NUS Downloader.

  * Seriously, there's no good reason to un-mod a Wii. You probably won't get more thorough help than this in doing so because no one does.
  
### I want to change a different SD Card / USB Device, can I just copy everything over?

  * Yes. You can use normal filecopy operations of your OS to move files from one location to the other, with no issue.
  
### Is there a way to transfer all the stuff on my Wii itself?

  * No. All stuff installed to the actual Wii memory will need to be re-installed.

----

## USB Loader GX

  These are the most common questions regarding USB Loader GX in which we get a lot of. If you can't find the answer here, you will most certainly be able to find it in the subreddit search.

### Can I use an SD Card?

  * For certain things, yes. However the Wii's SD Card slot, thanks to security encryption is considerably slower than the USB. So what does work works slower and with less compatibility than if you were using a USB device.

### My games aren't (showing up or loading) in USB Loader GX? Black Screen, Blank List, etc

  Here is a basic checklist:

  * Have you tried making sure they are checked to be displayed in USB Loader GX? You can get to this by pressing +, or make sure that your favorites aren't turned on.

  * Make sure your drive is plugged into the right port and being detected. It *needs* to be in the port closest to the outside of the device.
  
  * Make sure you're Wii has the correct cIOSes needed to run it. You can find that information [here](https://wii.guide/cios)
  
  * Ensure your hard drive is formatted in a way that can be read by whatever you are using. Wii games will work on NTFS, but the most compatible will be FAT32. You can format a drive in FAT32 from Windows by using the command line. DDG/Google.
  
  * Make sure your game files are in the proper directory structure. They are different for Wii/USBLoaderGX games, and Nintendont games. You can find information on how to do that in the links below:

    [nintendont](https://sites.google.com/site/completesg/backup-launchers/gamecube/nintendont)

    [usb loader gx](https://sourceforge.net/p/usbloadergx/wiki/Installation/)

  * Make sure USB Loader is configured properly. You can find information on doing so in the link above. Worst case scenario, delete your config. Start from scratch, remember what you change.

  * Are your images wbfs or iso? If they have the extension '.nkit' they will not work. Get a different image or learn to convert that one.
  
  * Last things to try are 'replacements'. Try a new game image, a different USB device, or SD card if possible. Yours might not be compatible, or sometimes not even good.
  
  * This information and more can be found in a user posted troubleshooting guide [here](https://www.reddit.com/r/WiiHacks/comments/dnfb81/usb_loader_gx_troubleshooting_guide/).

----

## Miscellaneous

  While the faq is growing, anything that doesn't have its own category will go here.

### How do I manage my virtual Wii game library?

  * Use [WiiBackupManager](http://www.wiibackupmanager.co.uk/WiiBackupManager_Build78.html) to get proper folder structure, gameID and to split large game files.

### How do I get WADs and Channel forwarders onto my Wii?

  * [YAWMM](https://github.com/FIX94/Some-YAWMM-Mod) is a great way to easily install wad files and channel forwarders.

### What Modded Wii Games can I play?

  * Check out our [useful links](https://wiihacks.bloodythorn.com/links) page.

----

## Helping out...

If you have any corrections, additions or suggestions, please message the moderators. We'd be glad to hear it.
