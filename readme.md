<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/KLOTZ_font_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/KLOTZ_font_bright.svg">
  <img alt="KLOTZ logo font" src="/docs/images/KLOTZ_font_bright.svg">
</picture>

# ZMK CONFIG FOR THE KLOTZ SPLIT KEYBOARD

[Here](https://github.com/GEIGEIGEIST/klotz) you can find the hardware files and build guide for the KLOTZ.

KLOTZ is a 34 key column-staggered split keyboard running [ZMK](https://zmk.dev/). It supports a low profile encoder and three status LEDs on every side.

![KLOTZ layout](/docs/images/KLOTZ_layout.svg)


## HOW TO USE

- fork this repo
- `git clone` your repo, to create a local copy on your PC (you can use the [command line](https://www.atlassian.com/git/tutorials) or [github desktop](https://desktop.github.com/))
- adjust the klotz.keymap file (find all the keycodes on [the zmk docs pages](https://zmk.dev/docs/codes/))
- `git push` your repo to your fork
- on the GitHub page of your fork navigate to "Actions"
- scroll down and unzip the `firmware.zip` archive that contains the latest firmware
- connect the left half of the KLOTZ to your PC, press reset twice
- the keyboard should now appear as a mass storage device
- drag'n'drop the `klotz_left-nice_nano_v2-zmk.uf2` file from the archive onto the storage device
- repeat this process with the right half and the `klotz_right-nice_nano_v2-zmk.uf2` file.


## KNOWN ISSUES

- ̶T̶h̶e̶ ̶e̶n̶c̶o̶d̶e̶r̶ ̶o̶n̶ ̶t̶h̶e̶ ̶s̶e̶c̶o̶n̶d̶a̶r̶y̶ ̶s̶i̶d̶e̶ ̶d̶o̶e̶s̶n̶'̶t̶ ̶w̶o̶r̶k̶ ̶y̶e̶t̶.̶ ̶T̶h̶i̶s̶ ̶i̶s̶ ̶a̶ ̶l̶i̶m̶i̶t̶a̶t̶i̶o̶n̶ ̶o̶f̶ ̶Z̶M̶K̶ 
  2023.6.18 페리퍼럴쪽 엔코더도 지원되게 바뀜
- The code for the status LEDs needs to be added.




