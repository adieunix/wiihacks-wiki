# Nintendont

Nintendont is a Wii mode homebrew to play Gamecube games on Wii and WiiU vWii.

Nintendont is not a modification or emulator. It's more like a bridge between an emulator and a virtual machine which runs Gamecube games natively.

For more information on Nintendont, you can read about it on the [GBATemp page](https://gbatemp.net/threads/nintendont.349258/) or their [GitHub page](https://github.com/FIX94/Nintendont)

## Installation
Nintendont doesn't have a package that is fully put together, it requires a little bit of manual labour.

1. Create a folder in your SD card's `apps` folder named `Nintendont` (yes it needs to be capitalized).
1. Download [loader.dol](https://github.com/FIX94/Nintendont/blob/master/loader/loader.dol?raw=true) and put it in the new `apps/Nintendont` folder as boot.dol.
1. Download the [meta.xml](https://github.com/FIX94/Nintendont/blob/master/nintendont/meta.xml?raw=true) file, and put that in `apps/Nintendont` as well.
1. Finally download and put the [icon.png](https://github.com/FIX94/Nintendont/blob/master/nintendont/icon.png?raw=true) file in to `apps/Nintendont`.

## Ripping your Gamecube Games
The old method to make Gamecube game rips is to use [CleanRip](https://wiibrew.org/wiki/CleanRip). It runs on both the Gamecube and the Wii. The only issue with using it for Gamecube games is that it doesn't put them in the correct location for Nintendont. It requires you to put your storage device in to your computer, then move and rename the image correctly.

The easiest method method is to use USB Loader GX to rip your Gamecube games. It will put them in the correct folder structure for Nintendont, and it still does a 1:1 copy like CleanRip.

## Gamecube Image Directory Structure
Your Gamecube games need to be on either your FAT32 formatted SD card or a FAT32 formatted storage device.

Create a folder names `games` on your storage device. Each game needs to be in their own folder, you then name the game EXACTLY as `game.iso` or `game.gcm` depending on their extension.

## _(Optional)_ Dump Gamecube BIOS for use with Nintendont
_Note: This is a completely optional thing. Nintendont runs perfectly fine without it. It's just if you want that nostalgic Gamecube start up when you use it._

You will require a couple of things: a working Gamecube, and a method to boot homebrew on said Gamecube. Different methods to do so can be found [here on the GC-Forever Wiki](https://www.gc-forever.com/wiki/index.php?title=Booting_Homebrew). The easiest way for people who already have a modified Wii is to use the `Game Save Exploits` that are shown on the [GC-Forever Wiki](https://www.gc-forever.com/wiki/index.php?title=Booting_Homebrew#Game_Save_Exploits).

1. Load up [Swiss](https://github.com/emukidid/swiss-gc).
1. Once you're loaded up on your storage device, press B to go to the bottom menu.
1. Press A on the eject looking button (first option)
1. In `Device Selection` scroll over to to `System` and press A.
1. Scroll down to `ipl.bin` and press A
  - If you get an error saying `Unknown File Type / Enable file management to manage this file`:
    1. Press B and go to settings (the gears) and press A to open that up.
    1. Under `Advanced Settings` you'll see an option for `File Management`, scroll down to it and press right to enable it.
    1. Keep pressing down until you've highlighted `Save & Exit`, press A.
    1. Wait until the settings screen closes. Press B to get back in to the file menu.
1. Press X to copy the file, select your storage device and then press X again to store it on the root of your SD card.
1. Wait a few seconds for it to copy over and then press A.

Now you're done on the Gamecube side and can turn it off. Put your SD card in to your computer and copy the `ipl.bin` file off of it. You'll need to rename it differently depending on the region of your Gamecube.

If you have a North American or NTSC system (outside of Japan) you'll name it `iplusa.bin`. If you have a PAL region system name it `iplpal.bin`. Finally, if you have a Japanese region Gamecube, then name it `ipljap.bin`.

Copy over your BIOS file to the root of your Gamecube game storage device (SD card or USB hard drive) and then in Nintendont's settings you need to make sure that `Skip IPL` is set to `No`. This does work with WiiU Gamecube injections made with [TechonMoon's WiiVC Injector Script](https://gbatemp.net/threads/release-wiivc-injector-script-gc-wii-homebrew-support.483577/) once the BIOS file is on your SD card and the setting is set not to skip.