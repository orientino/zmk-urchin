## Getting started
Create your own ZMK keymap for the Urchin starting from mine:

1) [Fork this repository](https://github.com/orientino/zmk-urchin/fork)
2) Enable actions on your fork. (click on the actions tab and enable it)
3) Edit the `config/urchin.keymap` file. (see [ZMK Codes](ps://zmk.dev/docs/codes))
4) When you push the changes an action will start and build your firmware. If the action is successful the file will be available in it's assets. (see [ZMK Docs](https://zmk.dev/docs/user-setup#installing-the-firmware)) 

Want to use my layout? Download the `firmware.zip` from the latest action run. Then check the [ZMK Docs](https://zmk.dev/docs/user-setup#installing-the-firmware) for instructions on how to flash it.

## Keymap design
This is an illustration to visualize the layout, which is created by considering the following principles:

- `vim` shortcuts require extensive usage of SHIFT
- `yabai/skhd` shortcuts are in the custom FUN layer

If you also use these tools, you can give it a try. The layout is complete while also being minimal with only 3 layers (+1 custom) and easily extendable.

```
/* 
 * BASE
 * ╭─────────────────────────────╮ ╭─────────────────────────────╮
 * |  Q  |  W  |  E  |  R  |  T  | |  Y  |  U  |  I  |  O  |  P  |
 * |  A  |  S  |  D  |  F  |  G  | |  H  |  J  |  K  |  L  | RET |
 * |  Z  |  X  |  C  |  V  |  B  | |  N  |  M  |  ,  |  .  |LSHFT|
 * ╰─────────────────╮ SY2 | CMD | | SPC | SY1 ╭─────────────────╯

 * SY1 (Symbols 1)
 * ╭─────────────────────────────╮ ╭─────────────────────────────╮
 * |  1  |  2  |  3  |  4  |  5  | |  6  |  7  |  8  |  9  |  0  |
 * |  (  |  )  |  {  |  }  |  "  | |  !  |  _  |  -  |  /  | BSPC|
 * |  <  |  >  |  [  |  ]  |  '  | |  ?  |  =  |  +  |  *  | DEL |
 * ╰─────────────────╮ LCTL| LALT| |     |     ╭─────────────────╯

 * SY2 (Symbols 2)
 * ╭─────────────────────────────╮ ╭─────────────────────────────╮
 * | ESC |  @  |  #  |  $  |  %  | |  ^  |  &  |  |  |  \  | HOME|
 * | CAPS| TAB |     |     |     | |  ~  |  :  |  ;  |ARROW| END |
 * |LSHFT|     |     |     |     | |  `  |     |ARROW|ARROW|ARROW|
 * ╰─────────────────╮     |     | | LALT| LCTL╭─────────────────╯

 * FUN (Functions): custom shortcuts
 * ╭─────────────────────────────╮ ╭─────────────────────────────╮
 * |     |     |     |     |     | |     |     |     |     |     |
 * |     |     |     |     |     | |     |     |     |     |     |
 * |     |     |     |     |     | |     |     |     |     |     |
 * ╰─────────────────╮     |     | |     |     ╭─────────────────╯
 */
```

## Credits
Thanks to my friend Duccio ([duckyb](https://github.com/duckyb)) for designing and helping me to build this beautiful keyboard. Thanks also to the ZMK community on Discord for their great support. Check the [Urchin's original repo](https://github.com/duckyb/urchin) to know more!
