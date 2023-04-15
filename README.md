# My QMK keymaps

This is the directory of my QMK keymaps. They are committed to my fork of QMK firmare which you can find [here](https://github.com/izevaka/qmk_firmware)

## Keymap links
* [Preonic](https://github.com/izevaka/qmk_firmware/tree/master/keyboards/preonic/keymaps/izevaka)
* [Lily58](https://github.com/izevaka/qmk_firmware/tree/master/keyboards/lily58/keymaps/izevaka)
* [StackOverflow Key](https://github.com/izevaka/qmk_firmware/tree/master/keyboards/massdrop/thekey/keymaps/izevaka)

## Instructions for future Igor
1. Install `qmk` - e.g. using Homebrew
```
brew install qmk
```
2. Configure qmk to point to the fork:
```
qmk clone izevaka/qmk_firmware ~/src/qmk_igor
```
3. Double check that your directory is set up correctly in qmk:
```
$> qmk config
user.qmk_home=/path/to/qmk_igor
# Update if needed:
$> qmk config user.qmk_home=/path/to/qmk_igor
```
4. Compile QMK:
```
qmk compile -kb lily58/rev1 -km izevaka
qmk compile -kb preonic/rev3 -km izevaka
qmk compile -kb massdrop/thekey -km izevaka-thekey
``` 
5. Flash using QMK toolbox