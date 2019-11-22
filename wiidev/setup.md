## Intro

  So you want to develop something for the Wii and ended up here.

  Below is my instructional on setting up a development environment for making Homebrew Wii applications.

  First we're going to start out with some basic requirements.

## Basic Knowledge

  Not trying to discourage anyone, but if you don't consider yourself proficient in programming and you're using this as your 'learn to program' goal, this is going to be tough. Real tough.

### C/C++

  First off, the language the libraries are written in is C. You can use C++ to code your applications, but if you don't know either, they are hard first-languages. I know from experience. They were my first and second languages.

### GNU GCC Compiler Suite

  Next, it uses the GNU toolchain to compile a binary from an x86 computer to the Wii's PowerPC environment. If you're not familiar with cross compiling, if you run into an issue related to it, it might be well more difficult to resolve.

  You'll want to be familiar with the GNU tool chain. The environment provided sets things up fairly simply by example. But if you ever want to deviate from that to say, setup a larger project, if you don't know about the GNU toolchain and how it links to libraries and the build files and generators available for it, you're going to be at a disadvantage.

### Posix Environment

  Lastly, it uses a Posix environment. Meaning that you are going to need to be in a unix-like or unix simulated environment. The easiest will of course be linux. If you are familiar with linux you'll have one hand up.

  If you are not a linux user and don't or can't change, then in Windows there are a few ways around this. MSYS and Cygwin are a couple of options. These extra layers are harder to setup than a native posix environment and add yet another element to troubleshoot should you have issues.

  OSX *is* a posix environment but it is heavily locked down by the manufacturer. I'm also not a Mac user so I can't really even start to tell you what might get in your way if you chose this route.

  Also setting up an IDE type environment is possible, but just another step in making a comfortable environment. It doesn't come with one. So far you'll be entering in code and stuff with a text editor, and manipulating files via the command-line. Sometimes you'll be working in command line-based text editors.

  You don't have to live like this, but you'll have to at least learn to operate like this.

## Still interested? Good.

### Into the Posix Environment

  First thing you are going to want to do is setup a posix environment. I'm not going to teach you how to do that. The Windows installer for the DevKitPro environment installs MSYS which will work just fine.

### Devkit Pro Setup

  I followed the [DevKitPro Getting Started](https://devkitpro.org/wiki/Getting_Started) article. It worked just fine for both windows and linux. It will have all the download links you need for your particular setup.

#### pacman for *nix platforms that don't have them.

  Note that for unix-like platforms you need to have 'pacman' the package manager to install devkitpro. If you're on *ubuntu like me, you'll need to follow the instructions on installing their pacman distro.

  Since ubuntu has a single-package manager philosophy, you won't get much help from the native community in this.

  [Newest Release Here](https://github.com/devkitPro/pacman/releases/tag/devkitpro-pacman-1.0.1).

  [Instruction Here](https://devkitpro.org/wiki/devkitPro_pacman).

  Otherwise if you're on Arch you can just follow the instructions on the same page for modifying your existing install.

#### Apologies for windows specific instructions:

  If you're on windows, all this should have been installed with the installer. But again, I'm a linux user and I didn't dwell on the windows process.

#### Environment Variables:

  Make sure the environment variables are set in your console startup (.bashrc, .zshrc, etc), as the software won't(shouldn't) compile with out it.

### Time to compile!

  By this time you've setup your environment. You've verified the proper package manager is installed, and you've used it to download the the proper dev package (wii-dev), or you've installed the installer for windows.

  You'll want to open a console. If you're in Windows, it *needs* to be a console for your simulated *nix environment such as MSYS or Cygwin.

  After everything is installed (in linux, should be true for windows too but I haven't verified) everything should be in your '/opt/devkitpro' directory.

  The entire installation should be isolated in this /opt/ dir. If you have your environment vars set, the compiler should have no issue finding it.

  From there, what *I* did, was I copied the 'examples' directory to my own location in my home dir, sudo chowned it, cd examples, and then 'make all'.

  I realize I breezed through this last step. This tutorial will not teach you how to work in a linux type environment. It would make it way too long and there are already tons of sources to learn.

  If you aren't familiar with 'ls, cd, sudo, chown' then you'll want to start by learning the basics of bash. This will also help you understand the Environment variables you set earlier.

  'make' is part of the GNU tool chain. You can learn about that anywhere. There are so many sources that listing one would insult your google-fu.

  If the examples build, you've just setup a Wii Homebrew development environment.

## Stay Tuned for what to do next to setup your own project!