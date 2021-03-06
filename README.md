# Blue Mood for micro

This is a port of [emacs's Blue Mood theme](https://emacsthemes.com/themes/blue-mood-theme.html) for the [micro](https://micro-editor.github.io/) text editor.

![Screenshot](https://raw.githubusercontent.com/blue-mood/blue-mood-everything/master/screenshots/micro-screenshot.png)

## Notes

This theme requires a terminal emulator that supports true color<sup>[1](#myfootnote1)</sup> and micro's true color mode to be enabled for it to look the intended way (the background color for example appears with a radically different color without true color). To enable true color for micro, write `export MICRO_TRUECOLOR=1` in your shell config file (e.g. .bashrc,.zshrc e.t.c).
Keep in mind that this port doesn't correspond 100% to the original emacs theme, due to the differences of micro's theming system in comparison to emacs's theming system.

## Installation & Activation

### Manual

1. Copy the bluemood-tc.micro file to the colorschemes directory: `~/.config/micro/colorschemes` (if the folder doesn't exist, create it) or `~/micro/colorschemes` .
2. Start up micro (or restart it if it was open when the file was copied over)
3. Enter the command mode (with CtrlE) and write `set colorscheme bluemood-tc`.

<a name="myfootnote1">1</a>: To check whether your terminal supports true color, paste the following on it and press enter: `printf "\x1b[38;2;255;100;0mTRUECOLOR\x1b[0m\n"`. If TRUECOLOR in orange letters shows up, true color is supported indeed (from [this gist](https://gist.github.com/XVilka/8346728), which also includes other tips for true color support in the terminal).
