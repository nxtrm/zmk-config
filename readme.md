<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/t_plus_logo_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/t_plus_logo_bright.svg">
  <img alt="t_plus logo font" src="/docs/images/t_plus_logo_bright.svg">
</picture>

# ZMK CONFIG FOR THE t_plus SPLIT KEYBOARD

[Here](https://github.com/GEIGEIGEIST/t_plus) you can find the hardware files and build guide.\
[Here](https://github.com/GEIGEIGEIST/qmk-config-t_plus) you can find the QMK config for the t_plus.

t_plus is a 38 key column-staggered split keyboard running [ZMK](https://zmk.dev/) or [QMK](https://docs.qmk.fm/). It's meant to be used with a SEEED XIAO BLE or RP2040.


![t_plus layout](/docs/images/t_plus_layout.svg)



## HOW TO USE

- fork this repo
- `git clone` your repo, to create a local copy on your PC (you can use the [command line](https://www.atlassian.com/git/tutorials) or [github desktop](https://desktop.github.com/))
- adjust the t_plus.keymap file (find all the keycodes on [the zmk docs pages](https://zmk.dev/docs/codes/))
- `git push` your repo to your fork
- on the GitHub page of your fork navigate to "Actions"
- scroll down and unzip the `firmware.zip` archive that contains the latest firmware
- connect the left half of the t_plus to your PC, press reset twice
- the keyboard should now appear as a mass storage device
- drag'n'drop the `t_plus_left-seeeduino_xiao_ble-zmk.uf2` file from the archive onto the storage device
- repeat this process with the right half and the `t_plus_right-seeeduino_xiao_ble-zmk.uf2` file.