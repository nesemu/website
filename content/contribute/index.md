---
title: "Contributing"
date: 2019-05-09T15:54:53-04:00
draft: false
---
# Getting the Code

NESEmu is hosted on [GitHub](https://github.com/nesemu/nesemu). To download the
code, **clone the repository**:

```bash
git clone https://github.com/nesemu/NESemu.git
```

# Building NESEmu

As a macOS Cocoa app, NESEmu builds in
[Xcode](https://developer.apple.com/xcode/). In the repository, open
`NESemu.xcworkspace` and build the `NESEmu` target:

```bash
cd NESemu
open NESemu.xcworkspace
```

Be sure to use Xcode 10 on macOS Mojave 10.14 or later.

# Submitting a Pull Request

Our preferred way to accept contributions is through pull requests on GitHub.
Start by **forking** your own copy of the NESEmu repository, **commit** your
changes there, and then **submit a PR** upstream.

A few guidelines to follow when submitting a pull request:

1. **Keep them small.** Multiple small pull requests are easier to review and
merge individually than one large, complex PR. A general rule of thumb is that a
PR should be no larger than a single new feature or bug fix.

2. **Submit and seek feedback early.** Don't spend a long time trying to perfect
your change before submitting a PR. Go ahead and submit so that the community
can looks at it and provide feedback. Speaking of feedback...

3. **Accept feedback.** You might be asked to change something about your PR.
Don't take it personally. Conforming to feedback is crucial to ensure that the
codebase remains cohesive and consistent and to keep the project moving in the
right direction.

# Ways to contribute

There are currently several areas that need improvement. Our backend emulation,
written in C++ and located in the `nes_lib` directory, is mostly complete, but
is currently lacking APU (Audio Processing Unit) emulation. This means that
NESEmu currently has no sound and is obviously a high priority right now as we
work towards making NESEmu a feature-complete emulator. We are also always
looking to add more mappers to our Gamepak emulator to support more titles!

Our frontend is written in Swift using Cocoa, and is far from complete. The main
missing feature right now is player-two controller input mappings, along with
gamepad input support. In addition, any improvements to the UI or overall user
experience are welcome!

Finally, the last major piece of development work is adding support for
savegames or save states. This will require significant work in both backend
(being able to load and export save files) and the frontend (a nice, polished UI
for creating and managing save states).

Of course, if you think of something else that needs improving or a new feature
we haven't thought of yet, please share! Also take a look at our [GitHub issue
tracker](https://github.com/nesemu/nesemu/issues) for an up-to-date list of
outstanding issues.

# Cross-Platform development

Currently the `APU` branch of our repository contains a separate, cross-platform
version of our app that builds using CMake and uses the SDL2 library to render
graphics and audio and read input. This was replaced in favor of the native
macOS version because of [a serious bug in the SDL2 library]
(https://github.com/nesemu/NESemu/issues/4). However, we are still open to the
possibility of creating a cross-platform version of our app, so if you're
interested in developing this further, let us know!
