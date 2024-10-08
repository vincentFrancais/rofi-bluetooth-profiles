<div align="center">
<h3>rofi-bluetooth-profiles</h3>
forked from https://github.com/ClydeDroid/rofi-bluetooth/

`bluetoothctl` `rofi` `dmenu`

</div>

## Installation

1. Install dependencies: [rofi](https://github.com/davatorium/rofi) and bluetoothctl (provided by `bluez-utils` in Arch)
2. Clone this repo
3. `cd rofi-bluetooth-profiles`
4. `./rofi-bluetooth`
1. (Optional) For easy access, add the script somewhere in your `$PATH`.

### Polybar configuration

`NOTE:` In order to properly display the bluetooth icon, you will need to use an iconic font in your bar, e.g. [Nerd Fonts](https://github.com/ryanoasis/nerd-fonts)

```
[module/bluetooth]
type = custom/script
exec = rofi-bluetooth --status
interval = 1
click-left = rofi-bluetooth &
```

### i3 keybinding

```
bindsym $mod+b exec --no-startup-id rofi-bluetooth
```

### Thanks for the inspiration!
- [ClydeDroid/rofi-bluetooth original rofi-bluetooth creator](https://github.com/nickclyde/rofi-bluetooth)
- [firecat53/networkmanager-dmenu](https://github.com/firecat53/networkmanager-dmenu)
- [x70b1's bluetoothctl polybar script](https://github.com/polybar/polybar-scripts/tree/master/polybar-scripts/system-bluetooth-bluetoothctl)
