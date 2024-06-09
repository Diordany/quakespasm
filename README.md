# QuakeSpasm

<img src="Misc/QuakeSpasm_512.png" width="128" />

[![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)

Forked from Ozkan Sezer's repository. Has some tweaks and hacks here and there that I like to use. For a more stable and cross-platform experience, please use the official QuakeSpasm repository instead.

## Official Repository Links

SOURCEFORGE: https://sourceforge.net/p/quakespasm/quakespasm/ci/master/tree/

GitHub Mirror: https://github.com/sezero/quakespasm

Releases: http://quakespasm.sourceforge.net/download.htm

[QuakeSpasm readme](Quakespasm.txt)

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

| Name               | Description                                                         |
|:-------------------|:--------------------------------------------------------------------|
| ***con_printcmd*** | *Prints the names of commands that are being executed in realtime.* |

### Commands

| Name       | Description                                                |
|:-----------|:-----------------------------------------------------------|
| ***exit*** | *Quits the game immediately (just like the quit command).* |