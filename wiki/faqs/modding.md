---
title: Wiki -> F.A.Q.s -> Modding
description: A wiki maintained by the r/WiiHacks community.
redirect_from: "/faqs/modding.md"
---

## Modding.

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

  * Wii compatibility is sporadic, but ones that outright don't work rarely than most people think. I'd suggest checking the [compatibility lists](https://www.wiihacks.org/links#storage-compatibility-lists) and if you plan on buying one, make sure the cost is negligible, or the place has a liberal return policy.

### Does anyone have a pre-setup SD/USB?

  * No, and asking for one would most likely violate rule #3 of the subreddit, and certainly violates rule #4.

### Well then, how do I setup my SD/USB storage?

   * This information is covered in several tutorials out there as well as the documentation for each piece of software.

   * [homebrew channel](https://wiibrew.org/wiki/Homebrew_Channel) -> for homebrew application installation.

   * [nintendont](https://github.com/FIX94/Nintendont) -> For your GameCube games.

   * [usb loader gx](https://sourceforge.net/p/usbloadergx/wiki/Installation/) -> For your Wii games.
   
   * Best information I could find on placing Wii games is on the [WiiBackupManager Site](http://www.wiibackupmanager.co.uk/) under the details for 'Simulated WBFS drives (FAT32/NTFS)' Of course if you can use this software it does it all for you.

#### Homebrew Applications

   * All applications for homebrew (dol, icon, meta.xml) will be installed in its corresponding apps directory.

   ```
   /apps
   /apps/usbloadergx/boot.dol
   /apps/usbloadergx/icon.png
   /apps/usbloadergx/meta.xml
   ```

   * Each program has different requirements for its configuration, and you need to *read* those instructions. For example;

   ```
   /apps
   /apps/snes9xgx/boot.dol
   /apps/snes9xgx/icon.png
   /apps/snes9xgx/meta.xml
   ```

   * And this will require a config directory ...

   ```
   /snex9xgx
   /snex9xgx/roms
   /snex9xgx/artwork
   ```

#### Wii Games for USBLoaderGX/WiiFlow/etc.

   * Additional information can be found on the [Official Support Thread on GBATemp](https://gbatemp.net/threads/usb-loader-gx.149922/). As well as searching everywhere as it's a commonly asked question.

   * If you can, use [WiiBackupManager](http://www.wiibackupmanager.co.uk/). If you can't, read the blurb under the details of 'Simulated WBFS drives (FAT32/NTFS)' and go download [Wit Tools](https://wit.wiimm.de/) for anything else it does.

   * Wii games must be an ISO or WBFS. Nkit images will *not* work with loaders currently.

   * The SD/USB card that you put them on must be either NTFS or Fat32. If you choose NTFS, realize that other pieces of homebrew might not recognize the partition, such as Nintendont. If you choose Fat32, realize that all disc images over 4gb will need to be split.

   * Images can be converted to and fro, and split with the numerous tools that are out there to do so. I recommend [WIT](https://wit.wiimm.de/).

   * Images should be named as per their name, and [ID](https://www.gametdb.com/Wii/List), with its corresponding extension (iso OR wbfs).

   ```
   Final_Fantasy_Fables-Chocobos_Dungeon_R7FEGD.iso
   ```

   * The name is optional. The game could just be named the ID.
   
   ```
   R7FEGD.wbfs
   ```

   * Images should be placed in a directory named wbfs off of root.

   ```
   /wbfs/Final_Fantasy_Fables-Chocobos_Dungeon_R7FEGD.iso
   ```

#### Nintendont - GameCube Games

   * Games can be in ISO, GCM, WBFS, or even NKit support has been verified.

   * There is no need for anything additional in this section as the [Nintendont Github](https://github.com/FIX94/Nintendont) covers it as well as you can. Please read the README.md under the section 'Quick Installation'.
   
### How do I know the current mod/cios state of my Wii?

  * Currently [SysCheck](http://www.hacksden.com/downloads.php?do=file&id=149) is recommended. Though be warned, there are certain kit-installers that can change your IOSes without changing the version number, thereby preventing your Wii from being modified. 
  * ["The installer tells me that it couldn't find a vulnerable IOS or something? What's that about?"](http://hbc.hackmii.com/faq/)

### I've botched the process, but my Wii still seems to work, what do I do?

  * To answer a common question on botched installs; NO you do not have to undo anything. As long as your Wii is still (mostly) functional, find some help, start the modding process over. You (almost) never need to undo what you've already done.

### Can I Un-MOD my Wii? Will formatting it remove the mods?

  * Sure. However first warning; you're looking at a procedure far more complex than what you did to mod your Wii.

  * Formatting the Wii will only remove user data. Removing/deleting the SD Card or USB Device will remove all homebrew and games.

  * If you can; updating the Wii might remove *most* of the modified software. Been wanting to make that jump from 4.1 to 4.3? Now's your chance. Just fair warning, this has the potential to brick your Wii.

  * If you were lucky enough to not be able to use an upgrade, you'll want to download all of the stock IOS and replace all of the modified ones with originals. Of course you'll still need your homebrew to do this with... The suggested tool would be the NUS Downloader.

  * Seriously, there's no good reason to un-mod a Wii. You probably won't get more thorough help than this in doing so because no one does. However if you insist, please direct your questions toward GBATemp, as these posts never go anywhere in r/WiiHacks.

### Can I update my mod? Or, I just bought a modded Wii, what do I do?

  * As stated before: Factory reset will clear out the user data, not the mods. Do it if you don't want what is on there. It might remove the HBC and you'll have to re-run the hack.
  * Clearing the SD card will remove all custom homebrew not installed on the Wii.
  * Realistically you'll want to just remove anything you don't want, and update anything you want to keep.
  * Update the cIOS via the recommended guide, and update any homebrew software it's running to the latest version.

### I want to change a different SD Card / USB Device, can I just copy everything over?

  * Yes. You can use normal filecopy operations of your OS to move files from one location to the other, with no issue.
  
  * If you're moving to an SD Card remember that USB Loader GX will have to be replaced with something that will play Wii games off a SD Card.
  
### Is there a way to transfer all the stuff on my Wii itself?

  * No. All software installed to the actual Wii memory will need to be re-installed.
