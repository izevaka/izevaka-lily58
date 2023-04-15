# Igor's Lily58 layout

This is intended to be used a submodule in my fork of [qmk_firmware](https://github.com/izevaka/qmk_firmware).

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
``` 
5. Flash using QMK toolbox