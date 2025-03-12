# Better-Control 🛠️ 
A gtk themed control panel for linux 🐧

<img src="https://github.com/user-attachments/assets/791074ba-466a-4f5d-80f4-1d1c71d795d1" width="500" />

This project is still under development , contriubutions such as ideas and feature requests towards project and testers are welcome.

# How to Install? ✅ 
before install make sure u have `git` and `base-devel` installed

## Dependencies

- GTK 4 (for the UI)
- NetworkManager (for managing Wi-Fi & Ethernet)
- BlueZ & BlueZ Utils (for Bluetooth support)
- PipeWire Pulse (for audio control)
- Brightnessctl (for screen brightness control)
- Python Libraries: python-gobject and python-pydbus and python3

### Arch Based
Arch users dont need to do all this installation processes, 

If you use `yay` then:

```yay -S better-control-git```

If you use `paru`then:

```paru -S better-control-git```

### Debian Based
```sudo apt update && sudo apt install -y libgtk-4-dev network-manager bluez bluez-utils pipewire-pulse brightnessctl python3-gi python3-dbus python```

### Fedora Based
```sudo dnf install -y gtk4 NetworkManager bluez bluez-utils pipewire-pulse brightnessctl python3-gobject python3-dbus python```

### Void Linux
```sudo xbps-install -S gtk4 NetworkManager bluez bluez-utils pipewire-pulse brightnessctl python3-gobject python3-dbus python```

### Alpine Linux
```sudo apk add gtk4 networkmanager bluez bluez-utils pipewire-pulse brightnessctl py3-gobject py3-dbus python```


## After you get the dependencies 
```
git clone https://github.com/quantumvoid0/better-control
cd better-control
sudo make install
sudo rm -rf ~/better-control

```
# How to uninstall? ❌

For arch users who installed through AUR do this to uninstall `sudo pacman -Rns better-control-git`

```
git clone https://github.com/quantumvoid0/better-control
cd better-control
sudo make uninstall
sudo rm -rf ~/better-control

```

# Compatability 📄
I have only tested this on Arch Linux with Hyprland so testers are welcome to test it out and share their review in discussions/issues. This should work on all distros (if u tested it pls leave a comment for any issues)

Probably will work on the stuff below 
| **Category**         | **Requirements**                                                                 |
|-----------------------|----------------------------------------------------------------------------------|
| **Operating System**  | Linux                                                                            |
| **Distributions**     | Arch based,Fedora Based,Debian Based,NixOS,Void,Alpine                                                            |
| **Desktop Environments** (might work) | GNOME, XFCE, KDE Plasma (with GTK support), LXDE/LXQT, etc.                  |
| **Window Managers**   | Hyprland (tested), Sway, i3, Openbox, Fluxbox, etc.                             |
| **Display Protocol**     | Wayland (recommended), X11 (partial functionality)                               |

# For WM users ✨
make it so that `control` runs as a floating window to make it look cool if u want

hyprwm example
```
windowrulev2 = float, class:control
windowrulev2 = opacity 0.5 0.5,class:control
```
