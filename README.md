# QuakeSpasm

<img src="Misc/QuakeSpasm_512.png" width="128" />

[![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)

Forked from Ozkan Sezer's repository. Has some tweaks and hacks here and there that I like to use. For a more stable and cross-platform experience, please use the official QuakeSpasm repository instead.

## Official QuakeSpasm Links

[Releases](http://quakespasm.sourceforge.net/download.htm)

[SOURCEFORGE Repository](https://sourceforge.net/p/quakespasm/quakespasm/ci/master/tree/)

[GitHub Mirror Repository](https://github.com/sezero/quakespasm)

[Readme](https://github.com/sezero/quakespasm/blob/master/Quakespasm.txt)

I'll try to keep the `upstream` branch up to date with the official repository.

## Building & Running

If you insist on building this version of QuakeSpasm, run the following:

```
git clone https://github.com/Diordany/quakespasm.git
cd quakespasm/Quake
make
```

Then run QuakeSpasm with:

```
./quakespasm
```

To clean the build, run:

```
make clean
```

This version enables SDL2 by default. To use SDL-1.2, run:

```
make USE_SDL2=0
```

To include debug symbols, run:

```
make DEBUG=1
```

To enable user directory support, run:

```
make DO_USERDIRS=1
```

## Custom CVars & Commands

Here's an overview of custom CVars and commands that have been included in this version:

### CVars

| Name                | Description                                                                                  |
|:--------------------|:---------------------------------------------------------------------------------------------|
| ***con_printcmd***  | *Prints the commands that are being executed in realtime.*                                   |
| ***host_intruder*** | *Resets the player inventory on every level (more specifically it uses the `map` command instead of `changelevel` to switch levels). This is inspired by Dusk's intruder mode.*      |
| ***host_loopmap***  | *Makes maps loop back on themselves (uses restart) during exectution of the changelevel command (at exit).* |

### Commands

| Name       | Description                                                |
|:-----------|:-----------------------------------------------------------|
| ***exit*** | *Quits the game immediately (just like the quit command).* |