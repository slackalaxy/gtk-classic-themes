# Clearlooks-classic-deepsky-0.1 (GTK2 + GTK3 + GTK4)

GTK3 and GTK4 port of the GTK2 "Clearlooks-DeepSky" theme from the original 2005 Clearlooks engine (clearlooks 0.6.2).
Same method as Clearlooks-classic-quicksilver: colours come from the engine's own shade() maths applied to the
theme's gtkrc palette; details that could be measured (scrollbar, menus, tabs, paned handle) were taken from
GTK2 screenshots of Quicksilver and scaled to this palette, so small differences from the real GTK2 theme
are possible. "classic" distinguishes these from the later Gummy-style Clearlooks.

Install: copy the `Clearlooks-classic-deepsky-0.1` folder to `~/.themes/` and select it as the GTK theme.
GTK4: libadwaita applications ignore third-party themes; GTK4 has no scrollbar stepper buttons.

## GTK2

`gtk-2.0/gtkrc` is the unchanged `Clearlooks-DeepSky` gtkrc from the original clearlooks-0.6.2 tarball. It needs a "clearlooks"
GTK2 engine installed (the engine from clearlooks 0.6.2 or the later gtk-engines).
