# OpenJK

OpenJK is an effort by the JACoders group to maintain and improve the game engines on which the Jedi Academy (JA) and Jedi Outcast (JO) games run on, while maintaining *full backwards compatibility* with the existing games. *This project does not attempt to rebalance or otherwise modify core gameplay*.

Our aims are to:
* Improve the stability of the engine by fixing bugs and improving performance.
* Provide a clean base from which new JO and JA code modifications can be made.
* Make available this engine to more operating systems. To date, we have ports on Linux and OS X.

Currently, the most stable portion of this project is the Jedi Academy multiplayer code, with the single player code in a reasonable state.

Rough support for Jedi Outcast single player is also available, however this should be considered heavily work in progress. This is not currently actively worked on or tested. OpenJK does not have Jedi Outcast multiplayer support.

Please use discretion when making issue requests on GitHub. The [JKHub sub-forum](http://jkhub.org/forum/51-discussion/) is a better place for support queries, discussions, and feature requests.

[![IRC](https://img.shields.io/badge/irc-%23JACoders-brightgreen.svg)](http://unic0rn.github.io/tiramisu/jacoders/)
[![Forum](https://img.shields.io/badge/forum-JKHub.org%20OpenJK-brightgreen.svg)](http://jkhub.org/forum/51-discussion/)

[![Coverity Scan Build Status](https://scan.coverity.com/projects/1153/badge.svg)](https://scan.coverity.com/projects/1153)

| Windows | OSX | Linux x86 | Linux x64 |
|---------|-----|-----------|-----------|
| [![Windows Build Status](http://jk.xd.cm/badge.svg?builder=windows)](http://jk.xd.cm/builders/windows) | [ ![OSX Build Status](http://jk.xd.cm/badge.svg?builder=osx)](http://jk.xd.cm/builders/osx) | [ ![Linux x86 Build Status](http://jk.xd.cm/badge.svg?builder=linux)](http://jk.xd.cm/builders/linux) | [ ![Linux x64 Build Status](http://jk.xd.cm/badge.svg?builder=linux-64)](http://jk.xd.cm/builders/linux-64) |

## License

[![License](https://img.shields.io/github/license/JACoders/OpenJK.svg)](https://github.com/JACoders/OpenJK/blob/master/LICENSE.txt)

OpenJK is licensed under GPLv2 as free software. You are free to use, modify and redistribute OpenJK following the terms in LICENSE.txt.

## For players

To install OpenJK, you will first need Jedi Academy installed. If you don't already own the game you can buy it from online stores such as [Steam](http://store.steampowered.com/app/6020/), [Amazon](http://www.amazon.com/Star-Wars-Jedi-Knight-Academy-Pc/dp/B0000A2MCN) or [GOG](https://www.gog.com/game/star_wars_jedi_knight_jedi_academy).

Installing and running OpenJK:

1. [Download the latest build](http://builds.openjk.org) for your operating system.
2. Extract the contents of the file into the Jedi Academy `GameData/` folder. For Steam users, this will be in `<Steam Folder>/steamapps/common/Jedi Academy/GameData`.
*Note:* The archive might unzip into `install/JediAcademy/` and in there is all the data. Actually *this* data should be in `GameData/` folder.
3. Run `openjk.x86.exe` (Windows), `openjk.i386` (Linux 32-bit), `openjk.x86_64` (Linux 64-bit) or the `OpenJK` application (OS X), depending on your operating system.
The executable `openjk` is the multiplayer mode, `openjk_sp` is the single player/story mode and `openjkded` is a standalone server for multiplayer games.


**OS X Instructions**

If you have the Mac App Store Version of Jedi Academy, follow these steps to get OpenJK runnning under OS X:  

1. Download the latest SDL2 Framework from [libsdl.org](https://www.libsdl.org/download-2.0.php)
2. Extract the content or open the file and put `SDL2.framework` in `/Library/Frameworks/` or `/Users/<USER>/Library/Frameworks/`  If this directory does not exist, create it.
3. Extract the content of the OpenJK DMG ([Download the latest build](http://builds.openjk.org)) into the game directory `/Applications/Star Wars Jedi Knight: Jedi Academy.app/Contents/`
4. Run `openJK.app` or `openJK SP.app` 
5. Savegames, Config Files and Log Files are stored in `/Users/<USER>/Library/Application Support/OpenJK/`


## For Developers

### Building OpenJK
* [Compilation guide](https://github.com/JACoders/OpenJK/wiki/Compilation-guide)
* [Debugging guide](https://github.com/JACoders/OpenJK/wiki/Debugging)

### Contributing to OpenJK
* [Fork](https://github.com/JACoders/OpenJK/fork) the project on GitHub
* Create a new branch and make your changes
* Send a [pull request](https://help.github.com/articles/creating-a-pull-request) to upstream (JACoders/OpenJK)

### Using OpenJK as a base for a new mod
* [Fork](https://github.com/JACoders/OpenJK/fork) the project on GitHub
* Change the GAMEVERSION define in codemp/game/g_local.h from "OpenJK" to your project name
* If you make a nice change, please consider back-porting to upstream via pull request as described above. This is so everyone benefits without having to reinvent the wheel for every project.

### Deciphering buildbot's output
* Pick the build from the operating system builder you're interested in at the [builders](https://jk.xd.cm/builders) page.
* Click on stdio for the Steps to see the command executed and the result.
* The command is at the very top, the output starts below.

## Maintainers (in alphabetical order)

* Ensiform
* Razish
* Xycaleth

## Significant contributors (in alphabetical order)

* eezstreet
* exidl
* ImperatorPrime
* mrwonko
* redsaurus
* Scooper
* Sil
* smcv
