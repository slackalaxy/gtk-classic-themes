# Industrial-GTK4

GTK4 CSS port of the GTK2 Industrial theme/engine from gtk-engines 2.20.2 (sister of Industrial-GTK3).
Colours, border opacities, radii and shadows are taken from `themes/Industrial/gtk-2.0/gtkrc` and
`engines/industrial/src/industrial_style.c`. Derived from LGPL-2.1+ code (Red Hat, Ximian, Benjamin Berg).

## Install
    mkdir -p ~/.themes && cp -r Industrial-GTK4 ~/.themes/
    gsettings set org.gnome.desktop.interface gtk-theme 'Industrial-GTK4'
(or use your desktop's appearance settings, or run an app with `GTK_THEME=Industrial-GTK4 app`).

## Notes
- Apps built on libadwaita (many recent GNOME apps) ignore third-party GTK4 themes. Plain GTK4 apps
  (file chooser dialogs, many Xfce/MATE/third-party apps) use this theme.
- Classic always-visible scrollbars: put this in `~/.config/gtk-4.0/settings.ini`
      [Settings]
      gtk-overlay-scrolling=false
- GTK4 has no scrollbar arrow buttons, so unlike the GTK3 version there are none.
- Tested against GTK 4.14. Check/radio marks are PNGs.

## Notes

- GTK3: the file chooser sidebar and the Xfce panel / notification area use full-colour icons
  (`-gtk-icon-style: regular`) from your current icon theme instead of monochrome symbolic ones.
- Menu drop shadows are not part of the theme (GTK3 menus need compositor-specific tricks that can crop popups).

