---
title: "About"
date: 2019-05-09T15:55:34-04:00
draft: false
---

# Fast Lightweight NES Emulation for MacOS

What started as an ambitious project for a course at the University of Notre Dame has evolved into a fully functional open source project. NESEmu is a Fast, Lightweight Nintendo NES Emulator. Currently the backend is written in C++ while the front end is made specifically for MacOS written in a combination of Objective-C and Swift.

The emulator currently support games such as Donkey Kong, Super Mario Bros, The Legend of Zelda, Metroid, and more!

**More Games are being added all the time!** Check back on this website to keep track of game support progress!

# Ready to Get Started?

Read our installation instructions on the [Install page]({{< ref "contribute/install.md" >}})

# Features

**Completely Open Source and Built From Scratch**


*	Countless Hours were spend perfecting the C++ backend as to make a fast and lightweight NES Emulator
*	Custom Code Runs the front end utilizing modern Apple Technologies and Development Practices
*	This code is and always will be free to use, modify, and redistribute under the BSD3-Clause "New" License

**Run Your Favorite Old Time Games**

*	NESEmu supports many of the original classic titles you know and love such as **Legend of Zelda**, **Super Mario Bros**, and **More!**
*	Discover new favorites and be taken back to a simpler age!
*	Currently Supports Keyboard input mapping
*	Future support is coming for utilizing your favorite USB Controllers with the emulator
*	Currently the Games do not have sound but that will be one of the first things we fix in the coming months!

**Project Roadmap**

In the future the maintainers of this project have a clear roadmap for where to take this project starting with Emulating the NES APU. This is a difficult task that will take some time but once it is down will mark end of development of a fully featured emulator.

After this is done we would like to start adding more mappers and welcome any help on adding more NES mappers. The more mappers we add the more games we can support. Basically mappers are NES cartridge-specific chips that allows the cartridge to contain more memory than what the NES can physically address. They do this by swapping out memory banks so one address can actually be multiple different things depending on the state of the cartridge. Learn more about mappers [here](http://wiki.nesdev.com/w/index.php/Mapper).

Finally we know that we do not support at lot of the quirky behavior of the NES, as time goes on we would love to be able to start supporting this behavior so that we can support the most games possible!

# Learn More About Contributing!

Interested in learning more about how to contribute to this project and make it **even better!?**
[Click Here]({{< ref "contribute/index.md" >}})
