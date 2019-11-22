# emuNAND - neek2o
`emuNAND` is the term used for a few different consoles, including (but not limited to): Wii, 3DS / 3DSXL / 2DS / new 3DS / new 3DSXL / new 2DS, WiiU, and Switch.

emuNAND is the way of redirecting the internal storage of a console over to a different storage medium. In the case of the Wii, it can be to either to an SD card or USB hard drive. The main use of emuNAND for the Wii is to have your channels (WAD files) installed on to your storage device of choice, instead of limiting you to the 500MB of internal storage on your console.

The main benefit of using emuNAND over the SD card menu on the Wii is that it is not tied to the console. You can take your storage medium and put it in to another homebrew enabled console and boot in it. All of your saves (from WiiWare and Virtual Console games) are also kept within the emuNAND environment.

## Building the emuNAND
1. Download and launch [ModMii](http://code.google.com/p/modmii/downloads/detail?name=ModMii6.3.1.zip).
  - If you get an error when launching `modmii.exe`, look in the `support/` sub-folder and launch `modmii.bat`
1. Type `I Agree` and press _enter_.
1. Type `O` and press _enter_ to enter the options screen.
  - Find the `n2o` line. It should display **(Enabled)** at the end of the line. If not, type `n2o` then _enter_.
  - Find the `SSD` line. It should display **(Disabled)** at the end of the line. If not, type `SSD` then _enter_.
  - Press `S` and then _enter_ to save settings, then `M` and press _enter_ to go back to the main screen
1. Type `S` and _enter_ to go to sneek creation menu.
1. If you've Type `3` and _enter_ to both set up / install SNEEK as well as create your emulated NAND.
1. Type `1` and _enter_ to choose the newest version of neek2o.
1. Type `S` and _enter_. We just need to create it for SD use, as USB Loader GX doesn't need disc emulation.
1. When it asks you where to save the files, don't enter anything, just press enter and it will be saved to the `COPY_TO_SD` and `COPY_TO_USB` folders in the ModMii folder.
1. Enter in the correct region code for your system, and press _enter_. If you don't select the same region, you will need to either have a different Wiimote set up for the emuNAND or sync up your Wiimote every time.
1. Enter in `4.3` and press _enter_. There is really no reason to go with `4.1` or `4.2`.
1. It is your choice on if you'd like to install `Post Loader` on to your emuNAND.
1. Press `N` and _enter_. `cIOS249` is not needed right now.
1. Press `N` and _enter_. `NMM` is useless.
1. Press `N` and _enter_. `Priiloader` can cause it to not load.
1. Press `N` and _enter_. `WiiFlow` Forwarder Channel is not needed.
1. Enter the serial number for your Wii (it's on the bottom of the unit).
1. Press `N` and _enter_. Menu themes aren't for game loaders.
1. Press `N` and _enter_. You don't need any of the normally built in channels.
1. Add any WAD files that you'd like installed to the `<modmii>\temp\WAD` folder. They will install during the build step.
1. Press `Y` and _enter_ to start the build process.
1. Copy the files `COPY_TO_SD` on to your SD card.

## Setting up your new emuNAND in USB Loader GX
1. WIP (next up)