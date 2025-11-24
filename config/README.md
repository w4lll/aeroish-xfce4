# Configuration Files
A configuration file provided for this theme/setup. Picom config is optional, you can use it to match my setup animations.

Tested on: Arch Linux with XFCE 4.20

# Panel
The panel configuration that can make it look aero-ish.

<img width="1366" height="40" alt="image" src="https://github.com/user-attachments/assets/9b23ccbf-ac66-432a-9588-c2562f32c1ec" />


## Requirements
If one of these panel applets are not listed, please add/install these plugins:
- Docklike plugin (required for Windows 7-like taskbar icons).
- Whisker menu plugin (for the start menu).
- Application menu (if don't want to use whisker menu plugin, the orb already configured).

## Installation
1. Download the gtk-3.0 folder and put the contents of the files (gtk.css, orb-related image) on '~/.config/gtk-3.0'. If you have an exisiting gtk.css, rename it or put it somewhere safe if you want to restore the original gtk.css later.
2. Back up your current panel profile if needed.
3. Set the panel height to 40, and fixed icon size to 16.
4. If you're on a fresh install of xfce, delete the dock (Panel 2 or whatever the bottom panel/dock is if there are two panels).
5. Change the order of the panel applets like this:

<img width="377" height="654" alt="image" src="https://github.com/user-attachments/assets/a5f6cc58-51f5-4977-8902-7cdf63f94bf8" />

(Clipman is optional.)

6. Restart the panel (`xfce4-panel -r`).
7. Configure these applets:
- Docklike plugin (hold CTRL then select properties):
<img width="459" height="683" alt="image" src="https://github.com/user-attachments/assets/b3a365d3-c088-4e9d-b62a-0a9f71753875" />


- Whisker menu

<img width="593" height="571" alt="image" src="https://github.com/user-attachments/assets/55e07bef-34fc-43d7-a03f-ada3d20536ba" />
<img width="593" height="571" alt="image" src="https://github.com/user-attachments/assets/1bce5bd3-c469-4b03-9f79-b82bf1554eed" />


## Customization
1. Button styles are on the gtk.css.
2. You can edit or replace the orb files, change on gtk.css to your needs (e.g. filenames).
3. Change the background of the panel to your needs.
   > Note: panelbg.xcf is the panel background that you can use. The width of the provided image is 1366. Edit to your current screen width, make sure the dark area on the right part is on the right of the width you set, and stretch the "top separation" (I don't know what to call it) to your current width you set. This panel background image will be essential to make your setup more aero-ish, otherwise this is optional.

## Known Issues
1. No docklike button look when opening 2 or more applications (I can't find the docs for it, or I might missed something).
2. Limited sizing for tray applets or may appear spaced on this large height.
3. Cropped pulseaudio volume pop-up (can be fixed by modifying the 'pulseaudio-plugin box' margin to 0, but this makes the tray applets more spaced, see image down below for more clear context).
4. Whisker menu button background might turned to opaque black if the background opacity is set to 100.
5. Some icon buttons are not configured yet.
6. Whisker menu icon got cropped if the panel size is below 40.

Image for no. 3:

<img width="168" height="160" alt="image" src="https://github.com/user-attachments/assets/320c7628-8666-4b01-8dd8-f19a2c130a69" />
