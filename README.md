# FS Game System

FS Game System expands on the functionality provided by FS-UAE Launcher
and FS-UAE Arcade in combination with the
[OpenRetro.org game database](https://openretro.org) by supporting other
platforms in addition to Amiga/CDTV/CD32.

Using **FS-UAE** Arcade to launch non-Amiga titles may not make any sense
from a naming perspective. It is expected that a there will be a new project
name for the combined solution in the future (*). For now, you can use
FS-UAE Launcher/Arcade to manage also non-Amiga games.

(*) Possibly "OpenRetro Player" and/or "OpenRetro Arcade".

This is a dummy project which can be used to file bugs / issues against
FS Game Systems, for issues which does not belong to fs-uae,
fs-uae-launcher, or fs-uae-arcade projects. Specifically, it can be used
to file bugs for non-Amiga platform support in FS Game System. This project
also holds documentation for FS Game System (FSGS).

## Supported Systems (Platforms)

* **Amiga** (FS-UAE)
* **Amstrad CPC** (MultiEmu-FS `*`)
* **Arcade** (MultiEmu-FS `*`)
* **Amstrad CPC** (MultiEmu-FS)
* **Atari 2600** (MultiEmu-FS)
* **Atari 5200** (MultiEmu-FS)
* **Atari 7800** (MultiEmu-FS)
* **Atari ST** (Hatari-FS)
* **Commodore 64** (Vice-FS)
* **CD32** (FS-UAE)
* **CDTV** (FS-UAE)
* **DOS** (DOSBox-FS)
* **Game Boy** (Mednafen-FS)
* **Game Boy Color** (Mednafen-FS)
* **Game Boy Advance** (Mednafen-FS)
* **Master System** (Mednafen-FS)
* **Mega Drive** (Mednafen-FS)
* **Nintendo (NES)** (Mednafen-FS)
* **PlayStation** (Mednafen-FS)
* **Super Nintendo (SNES)** (Mednafen-FS)
* **TurboGrafx-16** (Mednafen-FS)
* **ZX Spectrum** (MultiEmu-FS)

`*` MultiEmu-FS is basically MAME/MESS, but renamed due to trademark

There is ongoing work to support more platforms.
See "Platforms in Development" for more information.

## How to Get Started

First of all, you need a recent version of FS-UAE Launcher (2.9.4dev2
or higher). You should always use the latest available development
version, as some games/platforms may depend on it.

In addition, you need one or more emulator plugins, depending on what
gaming platforms you want to use. See "Supported Systems". The plugins
should be extracted into your `Documents/FS-UAE/Plugins` directory or
similar (if you use the portable version, extract into `Plugins` inside
the portable directory). Plugins are available from
[http://fs-uae.net/devel/plugins/](http://fs-uae.net/devel/plugins/).

**You need to restart FS-UAE Launcher after adding new plugins.**

You can also download an all-in-one portable bundle with FS-UAE Launcher,
FS-UAE Arcade and all emulator plugins for x86-64:
* Linux, Windows and macOS combined (x86-64): [x86-64.tar.gz](https://www.dropbox.com/s/cz10mocy85q3ewc/x86-64.tar.gz?dl=0)
* Windows only (x86-64):
[Windows.zip](https://www.dropbox.com/s/9olzcp6w7hg0l1h/Windows.zip?dl=0)

You then need to add some config values in FS-UAE Launcher: Settings:
Advanced Settings in order to download information from the additional
game databases (you only need to include the lines you want):

    arcade_database = 1
    atari_database = 1
    a2600_database = 1
    a5200_database = 1
    a7800_database = 1
    c64_database = 1
    cpc_database = 1
    dos_database = 1
    gb_database = 1
    gba_database = 1
    gbc_database = 1
    nes_database = 1
    psx_database = 1
    smd_database = 1
    sms_database = 1
    snes_database = 1
    tg16_database = 1
    zxs_database = 1

When you next update the game database in FS-UAE Launcher, the new
platforms will be available. It can be a good idea to enable displaying
all games in FS-UAE Launcher: Settings: Game Database, so you can see
even the games you don't have.

Finally, you need to have the actual game files. This works like it does
for Amiga games; you need to configure FS-UAE Launcher to scan your
game collection using the File Database functions. FS-UAE Launcher will
happily find game files within .zip or .lha archives.

When you run the "Update File Database" function in FS-UAE Launcher,
recognized games should appear automatically.

Please note that some platforms require you to have system ROM files as
well. If a ROM file is missing, you'll get an error messag saying which
ROM file was not found when you try to start the game via FS-UAE Launcher.

## Common Keyboard Shortcuts

* <kbd>Alt+Q</kbd> (<kbd>Cmd+Q</kbd>) to quit the emulator.
* <kbd>Alt+W</kbd> (<kbd>Cmd+W</kbd>) for warp speed (some emulators)
* <kbd>Alt+M</kbd> (<kbd>Cmd+M</kbd>) to mute/unmute audio.
* <kbd>Alt+S</kbd> (<kbd>Cmd+S</kbd>) to take a screenshot.
* <kbd>Alt+G</kbd> (<kbd>Cmd+G</kbd>) to grab input (some emulators).
* <kbd>Alt+P</kbd> (<kbd>Cmd+P</kbd>) to pause/resume emulation.

Some keyboard shortcuts may not be implemented for all emulators yet.

## Notes for FS-UAE Launcher

When using FS-UAE Launcher, you are currently not able to choose
input devices for input ports. FS-UAE Launcher will auto-select any
joysticks identified, or use keyboard emulation as a fallback. If you
use FS-UAE Arcade instead, you'll be able to choose input devices before
starting a game.

## Notes for FS-UAE Arcade

## To-Do

* Functionality for storing save data (memory card, cartridge save data,
  save disks, etc) is currently disabled. This needs to be enabled again
  on a per-platform basis.
* Functionality for storing save states is currently disabled. This needs
  to be enabled again on a per-platform basis.
* Many platforms have rudimentary support, and needs more testing and
  polishing.
* Some platforms needs more work to support a greater range of games.
* To-Do: Add platform-specific to-dos.

## Platforms in Development

...
