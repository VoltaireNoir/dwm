# Functional dwm
#### A version of dwm that sucks-less

Suckless' [Dynamic Window Manager](https://dwm.suckless.org/) is a great piece of software in itself, however, due to the minimalist philosophy behind its development, dwm lacks so many important features that a tiling WM should have (for example: a system tray in status bar, abiltiy to move windows in the stack, ability to restart dwm, etc). The users are meant to add any functionality they like by applying the patches, but this can discourage a lot of new users as applying the patches can be a tedious process and sometimes even frustrating.

This version of aims to provide a version of dwm that ships with all the important patches which mostly include the ones that modify or add additional functionality and a couple that make the WM look clean and modern. This way the users can install dwm and have a usable setup ready in no time. It also comes with a configuration with sane defaults.

## Install
- Clone Repo
`git clone https://github.com/VoltaireNoir/dwm .dwm`
- Compile dwm
`cd .dwm && sudo make clean install`
- Add `exec dwm` to your xinitrc or if you use a Display Manager (a login manager), create `dwm.desktop` file in `/usr/share/xsessions/` with the following contents: 
  ```
  [Desktop Entry]
  Name=dwm
  Comment=Dynamic Window Manager
  Exec=dwm
  Type=Application
  ```

## Configure
- Edit `config.h` and save the changes.
- Compile dwm
- Restart dwm (mod+shift+r)

## Included Patches
- [Actual Fullscreen](https://dwm.suckless.org/patches/actualfullscreen/) 
  - Toggle fullscreen mode for windows/clients
- [Adjacent Tag](https://dwm.suckless.org/patches/adjacenttag/) 
  - Switch to adjacent tags with keyboard shortcuts
- [Always Center](https://dwm.suckless.org/patches/alwayscenter/)
  - Floating windows will always spawn in the center instead of being spawned in the top-left corner
- [Attach Below (toggleable)](https://dwm.suckless.org/patches/attachbelow/)
  - New clients are added below the active client instead of being added to the master stack (this behaviour can be toggled on/off using the shortcut mod+shift+tab or in the config file
- [Autostart](https://dwm.suckless.org/patches/autostart/)
  - Autostart programs by adding them to the `autostart.sh` or `autostart_blocking.sh` in `.dwm/` directory
- [Bar Height](https://dwm.suckless.org/patches/bar_height/)
  - Pick bar height or let dwm calculate it automatically for you
- [Cfacts](https://dwm.suckless.org/patches/cfacts/)
  - Resize individual tiled windows (changes can be reset with mod+shift+n)
- [Color Bar](https://dwm.suckless.org/patches/colorbar/)
  - Modify foreground or background colors of all status bar elements
- [EWMH Tags](https://dwm.suckless.org/patches/ewmhtags/)
  - "EWMH support for _NET_NUMBER_OF_DESKTOPS, _NET_CURRENT_DESKTOP, _NET_DESKTOP_NAMES, and _NET_DESKTOP_VIEWPORT, which allows for compatibility with other bars and programs that request workspace information"
- [Full Gaps](https://dwm.suckless.org/patches/fullgaps/)
  - Add gaps around the clients (can be controlled with keyboard shortcuts)
- [Move Resize](https://dwm.suckless.org/patches/moveresize/)
  - Move and resize floating windows
- [Move Stack](https://dwm.suckless.org/patches/movestack/)
  - Move tiled windows up or down in the stack (mod+shift+j/l)
- [Per Tag](https://dwm.suckless.org/patches/pertag/)
  - Enable per tag layouts
- [Remove Border](https://dwm.suckless.org/patches/removeborder/)
  - Remove border if only a single window is occupying the tiling space
- [Reset Layout](https://dwm.suckless.org/patches/resetlayout/)
  - Reset master stack horizontal size to default
- [Restart Sig](https://dwm.suckless.org/patches/restartsig/)
  - Restart dwm (especially useful after making changes and re-compiling)
- [Sys Tray](https://dwm.suckless.org/patches/systray/)
  - System tray for the built-in dwm status bar
