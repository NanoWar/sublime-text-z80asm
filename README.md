# Z80 ASM TI package for Sublime Text 2/3
Bundled with [FunkLibrary](https://github.com/NanoWar/FunkLibrary) and SPASM

---

## Product information

This plugin contains syntax definition for Z80 assembler language (targeting Texas Instruments calculators, mainly TI83+), code snippets, its own shiny color theme and build system.

---

## Installation

Simply copy the `z80asm-ti` directory to the Sublime Text `Packages` directory. Under Windows that would be in you User folder `...\AppData\Roaming\Sublime Text 3\Packages\`.
Go to the `Tools > Build System` menu and select the `z80asm-ti` item. Now you can press Ctrl+B to build the opened file or the project if there is a FunkLibrary config file (see FunkLibrary's readme).

You need to check out the spasm-funk (https://github.com/NanoWar/spasm-funk) submodule by typing:
When you already pulled the z80asm-ti repository:
* git submodule update --init

Or you initially clone z80asm-ti recursively with:
* git clone --recursive https://github.com/NanoWar/z80asm-ti.git

---

## Features

#### Color scheme

This plugin contains its own color scheme `z80asm-ti.tmTheme` based on Monokai theme. There are some `*.z80` scope selectors with specific colors for assembler tokens.


#### Build system

This package uses SPASM as assembler and FunkLibrary. If you want to compile with z80asm-ti and the automatic build system using `Ctrl+B`, you use FunkLibrary by default. You can use the menu to assemble with only SPASM or change the build script `z80asm-ti.sublime-build` in this package yourself.


#### Emulator support

Currently this plugin searches for an executable 'Wabbitemu.exe' in the current project's folder and runs it when there is also a file that end with *.8xk or *.8xp. You can modify this in the 'z80asm-ti.py' script.


#### Snippets

There are a few useful snippets that you can trigger by typing their name and pressing tab:

* --- Delimiter small
* === Delimiter big
* *** Delimiter block
* loop Loop with register b
* loopbc Loop with register bc


#### Help files

In the `z80Asm > Help` sub-menu you can find a few help files. Some of them are provided with the plugin, and you also can put your help file into `Packages/z80asm/helps/`, and it will appear in menu. There are maximum 10 files allowed.

Also, you can call a quick help panel by pressing F1 where you can do a search through opcodes/mnemonics/timings.

---

## Support

If you have a bug/feature request - please post it on the [issue tracker](https://github.com/NanoWar/sublime-text-z80asm-ti/issues).

---

## Thanks

* psb^hlw
* breeze
* introspec
* key-jee
* elf/2
* Sean Young

---

## Copyright and license

(c) 2013, psb^hlw
(c) 2015, NanoWar (owner of this fork)

Software is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
