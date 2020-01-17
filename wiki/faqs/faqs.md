---
title: Wiki -> F.A.Q.s
description: A wiki maintained by the r/WiiHacks community.
redirect_from: "/faqs/faqs.md"
---

## [Modding F.A.Q.](./modding.md)

  You can find the modding FAQ [here](./modding.md).

----

## Regarding the subreddit.

### My post keeps getting flagged for Rule #4, why?

  There are two types of posts that get flagged for Rule #4. Help requests or questions that are regularly asked are removed, as well as ones that ask vague questions and/or provide vague information.

  People are less likely to respond to a help request if the first thing they need to do is ask you to provide the proper information.

### How can I get my post to not get removed by Rule #4?

  Always research the issue in the forum before you post. 98% of all questions asked are asked and answered regularly. If your post was removed because of this, you really didn't need to post to begin with.

  Provide enough information for the person to troubleshoot your issue;

  * Your post should have a title that briefly, but accurately describes the issue.
  
  * In the body, included should be a full description of the issue.
  
  * Include your hardware setup. What Wii are you using? The model and size of SD and USB device is often relevant, include it too. Do you have an original Wiimote, or a motion plus?
  
  * Include your software setup. A syscheck is almost always helpful. Paste the results into a pastebin and include it in your body. Like [this](https://pastebin.com/agpxtvXz).
  
  * Include everything you've done up until that point including links to tutorials you've followed and try to describe the results as best as you can.
  
  * The more information you provide, the less chance of the post getting removed as well as the more chance you have of getting someone to help you resolve your issue.

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

    [nintendont](https://github.com/FIX94/Nintendont) -> For your GameCube games.

    [usb loader gx](https://sourceforge.net/p/usbloadergx/wiki/Installation/) -> For your Wii games.

  * Make sure USB Loader is configured properly. You can find information on doing so in the link above. Worst case scenario, rename your config so it will generate a new one.

  * Are your images wbfs or iso? If they have the extension '.nkit' they will not work. Get a different image or learn to convert that one.
  
  * Last things to try are 'replacements'. Try a new game image, a different USB device, or SD card if possible. Yours might not be compatible, or sometimes not even good.
  
  * This information and more can be found in a user posted troubleshooting guide [here](https://www.reddit.com/r/WiiHacks/comments/dnfb81/usb_loader_gx_troubleshooting_guide/).

### Ripping games using USB Loader GX isn't working.

  * USB Loader GX has a habit of stopping in the middle of a rip and never completing, if it works at all.

  * After this issue appearing in the subreddit numerous time, the general public consensus is to not use it to rip games. It doesn't do it reliably, or accurately.
  
  * Use [CleanRip](https://github.com/emukidid/cleanrip) instead. It's more recently maintained and works much better.

### Why is my [Crap](https://sites.google.com/site/completesg/backup-launchers/usb/crap) Forwarder not working in USB Loader GX?

  * USB Loader GX was recently updated and it broke Crap compatibility. 
  * Currently we have tested Crap forwarders on USB Loader GX v2.3.
  * If you can live without the features of the newer version, this is going to be the only way to get the Crap forwarders working.

#### References:

  https://www.reddit.com/r/WiiHacks/comments/efone1/usb_loader_gx_isnt_launching_through_my_crap_wads/

----

## Miscellaneous

  While the faq is growing, anything that doesn't have its own category will go here.
  
### Homebrew Browser

  * Don't use it. There's no support for it.
  
  * No? Don't ask for help on r/WiiHacks for it. We don't support it.

### How do I manage my virtual Wii game library?

  * Use [WiiBackupManager](http://www.wiibackupmanager.co.uk/WiiBackupManager_Build78.html) to get proper folder structure, gameID and to split large game files.

### How do I get WADs and Channel forwarders onto my Wii?

  * [YAWMM](https://github.com/FIX94/Some-YAWMM-Mod) is a great way to easily install wad files and channel forwarders.

### What Modded Wii Games can I play?

  * Check out our [useful links](https://www.wiihacks.org/links) page.

----

## Helping out...

If you have any corrections, additions or suggestions, please message the moderators. We'd be glad to hear it.
