# VNC

Control the steamdeck in desktop mode from a PC.

## Installation

1. Set a password for your user account if not already done.
2. `sudo steamos-readonly disable`
3. `sudo pacman-key --populate holo`
4. `sudo steamos-readonly enable`
5. `sh -c "$(curl -fsSL https://gist.githubusercontent.com/x43x61x69/9a5a231a25426e8a2cc0f7c24cfdaed9/raw/vnc_install.sh?$RANDOM)"`

This will create a folder on the Desktop containing helpful scripts.

## Auto-start on start up

Some people would recommend you to setup a system service to have VNC server start on startup automatically. But for the sake of simplicity, I would suggest set it up with the GUI:

1. `Application Launcher > System > System Settings > Startup and Shutdown > + Add… > Login Script.`
2. Select the “vnc_startup.sh” within the VNC folder on your desktop.

![image](https://github.com/user-attachments/assets/117f39aa-0b90-48fc-9ee8-22c8ff2482a1)

Of course, this is complete optional. You can always use the shortcuts to start/stop the VNC server manually.

## Reinstalling

VNC will most likely be uninstalled when upgrading SteamOS.

1. `sudo steamos-readonly disable`
2. `sudo pacman-key --populate holo`
3. `sudo steamos-readonly enable`
4. Launch `~/Desktop/VNC/Reinstall VNC.desktop`
