# Friday Night Funkin' Plus

This is the repository for Friday Night Funkin' Plus, a modification of the latest source code of Friday Night Funkin' that brings in v0.2.8 features and improvements, without Week 7.

- View the original source code here: https://github.com/ninjamuffin99/Funkin
- Play the Ludum Dare prototype here: https://ninja-muffin24.itch.io/friday-night-funkin
- Play the Newgrounds version here: https://www.newgrounds.com/portal/view/770371
- Support the original on the itch.io page: https://ninja-muffin24.itch.io/funkin
- View progress of The Full Ass Game on its Kickstarter page: https://www.kickstarter.com/projects/funkin/friday-night-funkin-the-full-ass-game

## Friday Night Funkin' Plus Credits

- [M&M](https://github.com/ActualMandM) - Main Programmer
- [Netyasha Roozi](https://github.com/NetyashaRoozi) - Ridge (SiIvaGunner Rip)

## Friday Night Funkin' Credits / shoutouts

- [ninjamuffin99](https://twitter.com/ninja_muffin99) and [MtH](https://twitter.com/emmnyaa) - Programmer
- [Phantom Arcade](https://twitter.com/phantomarcade3k) and [evilsk8r](https://twitter.com/evilsk8r) - Art
- [Kawai Sprite](https://twitter.com/kawaisprite) and [bassetfilms](https://twitter.com/Bassetfilms) - Musician

This game was made with love to Newgrounds and its community. Extra love to Tom Fulp.

## Build instructions

### Installing the Required Programs

First, you'll need to install [Haxe](https://haxe.org/download/), [HaxeFlixel](https://haxeflixel.com/documentation/install-haxeflixel/), and [Git](https://git-scm.com/downloads).

Other installations you'd need are the additional libraries. Currently, these are all of the things you need to install:
```
haxelib install polymod
haxelib git discord_rpc https://github.com/Aidan63/linc_discord-rpc
```

You should have everything ready for compiling the game! Follow the guide below to continue!

### Compiling game
NOTE: If you see any messages relating to deprecated packages, ignore them. They're just warnings that don't affect compiling.

Once you have all those installed, it's pretty easy to compile the game. You just need to run `lime test html5 -debug` in the root of the project to build and run the HTML5 version.

To run it on your desktop (Windows, Mac, Linux), it can be a bit more involved. You ***MUST*** be on the platform you are compiling for.

For Windows, you need to install Visual Studio Community 2019. While installing VSC, don't click on any of the options to install workloads. Instead, go to the individual components tab and choose the following:
* MSVC v142 - VS 2019 C++ x64/x86 build tools
* Windows SDK (10.0.17763.0)

Once that is done you can open up a command line in the project's directory and run `lime test windows -debug`.

For Linux, you can either compile via WSL 2.0 (Windows) or on a Linux kernel. You only need to open a terminal in the project directory and run `lime test linux -debug`.

For Mac, install Xcode and `lime test mac -debug` *should* just work; if not, the internet surely has a guide on how to compile Haxe stuff for Mac.

Once the command finishes (it takes a while, even on a higher end PC), Friday Night Funkin' will boot up automatically.

### Additional guides
- [Command line basics](https://ninjamuffin99.newgrounds.com/news/post/1090480)
