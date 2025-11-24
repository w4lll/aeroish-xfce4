Aero-ish XFCE Panel
An XFCE4 panel theme that tried it's best to look like Windows 7 taskbar. This setup is unfinished, you might encounter some of issues that I may have or never experienced.

Tested on: Arch Linux with XFCE 4.20.

Requirements:
1. Applets
If one of these panel applets are not listed, please add/install these plugins:
- Docklike plugin (required for Windows 7-like taskbar icons).
- Whisker menu plugin (for the start menu).
- Application menu (if don't want to use whisker menu plugin, the orb already configured).

Note: panelbg.xcf is the panel background that you can use. The width of the provided image is 1366. Edit to your current screen width, make sure the dark area on the right part is on the right of the width you set, and stretch the "top separation" (I don't know what to call it) to your current width you set. This panel background image will be essential to make your setup more aero-ish, otherwise this is optional.

Installation:
1. Download the gtk.css and orb-related files and put these files on '~/.config/gtk-3.0'. If you have an exisiting gtk.css, rename it.
2. Back up your current panel profile if needed.
3. Set the panel height to 40, and fixed icon size to 16.
4. If you're on a fresh install of xfce, delete the dock (Panel 2 or whatever the bottom panel is).
5. Change the order of the panel applets like this:
[Whisker menu] [Docklike taskbar] [Separator (expand)] [Separator] [Status tray plugin] [Power manager plugin] [PulseAudio plugin] [Clock] [Show desktop]
If you want to make it the same as my current setup:
[Whisker menu] [Docklike taskbar] [Separator (expand)] [Separator] [Status tray plugin] [Power manager plugin] [PulseAudio plugin] [Clipman] [Clock] [Show desktop]
6. Restart the panel (xfce4-panel -r).
7. Configure these applet:
- Docklike plugin (hold CTRL then select properties):
> Active indicator style: None
> Inactive indicator style: None
> Force icon size: 32.
- Whisker menu:
>> General
> Show as list
> Check Show application tooltips 
> Uncheck Show application descriptions
> Application icon size: Small
> Category icon size: None
> Menu width: 400
> Menu height: 620
> Background opacity: 50%
>> Appearance
> Check Position search entry to bottom
> Check Position commands next to search entry
> Profile: Square Picture
- Application menu (if not using whisker menu):
> Uncheck Show button title

Customization:
1. Customizations like buttons are on the gtk.css.
2. You can edit or replace the orb files, change on gtk.css to your needs (e.g. filenames).
3. Change the background of the panel to your needs.

Known Issues:
1. No docklike button look when opening 2 or more applications (I can't find the docs for it, or I might missed something).
2. Limited sizing for tray applets or may appear spaced on this large height.
3. Cropped pulseaudio volume pop-up (can be fixed by modifying the 'pulseaudio-plugin box' margin to 0, but this makes the tray applets more spaced).
4. Whisker menu button background might turned to opaque black if the background opacity is set to 100.
5. Some icon buttons are not configured yet.
6. Whisker menu icon got cropped if the panel size is below 40.