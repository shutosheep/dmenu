# Shuto's build of dmenu (dynamic menu for X)

This is my personal [dmenu](https://tools.suckless.org/dmenu/) fork with some patches applied.

## Features

+ `-F` to enable fuzzy-matching
+ `-P` for password mode to hide user input

## Installation

```
git clone https://github.com/shutosheep/dmenu.git
cd dmenu
cp config.def.h config.h
sudo make clean install
```

Configuration is done with `config.h`. Default values are stored in `config.def.h`.

## Install `libxft-bgra` for emoji

This build of dmenu does not block color emoji so you must install `libxft-bgra` which fixes problem rendering color emojis. If you didn't install it and try rendering color emojis, it will crash upon trying to render one. If you are using arch linux based distribution, you can use [AUR](https://aur.archlinux.org/packages/libxft-bgra).

## Applied patches

+ [fuzzymatch](https://tools.suckless.org/dmenu/patches/fuzzymatch/)
+ [password](https://tools.suckless.org/dmenu/patches/password/)
