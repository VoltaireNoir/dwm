# Functional DWM
#### A version of DWM that sucks-less

The Suckless' [Dynamic Window Manager](https://dwm.suckless.org/) is a great piece of software in itself, however, due to the minimalist philosophy behind it's development, DWM lacks so many important features that a tiling WM should have. The users are meant to add any functionality they like by applying the patches, but this can discourage a lot of new users as applying the patches can be a tedious process.

This version of aims to provide a version of DWM that ships with all the important patches which mostly include the ones that modify or add additional functionality and a couple that make the WM look clean and modern. This way the users can install dwm and have a usable setup ready in no time.

## Installation
- Clone Repo
`git clone https://github.com/VoltaireNoir/dwm .dwm`
- Compile DWM
`cd .dwm && sudo make clean install`

## Configure
- Edit `config.h` and save the changes.
- Compile dwm
- Restart dwm (mod+shift+r)

## Included Patches
- [Actual Fullscreen](https://dwm.suckless.org/patches/actualfullscreen/)
- [Adjacent Tag](https://dwm.suckless.org/patches/adjacenttag/)
- [Always Center](https://dwm.suckless.org/patches/alwayscenter/)
- [Attach Below (toggleable)](https://dwm.suckless.org/patches/attachbelow/)
- [Autostart](https://dwm.suckless.org/patches/autostart/)
- [Bar Height](https://dwm.suckless.org/patches/bar_height/)
- [Cfacts](https://dwm.suckless.org/patches/cfacts/)
- [Color Bar](https://dwm.suckless.org/patches/colorbar/)
- [EWMH Tags](https://dwm.suckless.org/patches/ewmhtags/)
- [Full Gaps](https://dwm.suckless.org/patches/fullgaps/)
- [Move Resize](https://dwm.suckless.org/patches/moveresize/)
- [Move Stack](https://dwm.suckless.org/patches/movestack/)
- [Per Tag](https://dwm.suckless.org/patches/pertag/)
- [Remove Border](https://dwm.suckless.org/patches/removeborder/)
- [Reset Layout](https://dwm.suckless.org/patches/resetlayout/)
- [Restart Sig](https://dwm.suckless.org/patches/restartsig/)
- [Sys Tray](https://dwm.suckless.org/patches/systray/)
