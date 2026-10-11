# Clearlooks-classic-quicksilver-0.1 (GTK2 + GTK3 + GTK4)

GTK3 and GTK4 recreation of the GTK2 "Clearlooks-Quicksilver" theme, built for the original 2005 Clearlooks engine
(clearlooks 0.6.2: `clearlooks_draw.c`, `clearlooks_style.c`, `support.c` and
`themes/Clearlooks-Quicksilver/gtk-2.0/gtkrc`). It is *not* derived from the later Gummy-style Clearlooks:
every colour comes from the old engine's own `shade()` maths applied to the Quicksilver palette
(bg 0.95 grey, buttons #f0f1f2, selection #5598d7, notebook 0.93 grey, white menus, #ffffbf tooltips).

Install: copy the `Clearlooks-Quicksilver` folder to `~/.themes/` and select it as the GTK theme.

What is taken from the engine:
- buttons: 4-point gradient (bg x1.055 / x1.005 / x0.98 / x0.91), border bg x0.5 -> x0.62, white line inside the
  top/left, shade[1] inside the bottom/right, 1px "inset" ring outside; pressed = bg[ACTIVE] gradient, darker border
- entries: x0.62 border, light line inside, spot[2] border + spot[0] ring on focus
- scrollbars: grey slider (light -> dark across its width) with three dark/white grip line pairs, grey steppers
  with chevron arrows on the steppers (solid triangles elsewhere), shade[2] trough with shade[5] sides, single 1px line against the frame
- check/radio marks: the engine's own bitmaps (bits.c), cut to the indicator interior
- tabs: inactive = bg[ACTIVE] with lighter top; selected = lighter top + 3px selection-colour stripe on the outer edge
- menus: white, shade-0.5 border; items = selection -> selection x0.8 gradient with white text; flat grey menubar
- progress bars: spot colour gradient with solid diagonal candy stripes
- scales: 5px trough, spot-coloured fill, plain rounded slider without grip
- tree views: gradient selection (grey while the list is not focused), column headers with dark/white separators
- paned handle: two columns of dark/white dots (as drawn by your GTK2 runtime)

Not done / approximations:
- the outer "inset" ring on buttons and entries is drawn as a pair of 1px outer shadows (dark above, light below)
- candy stripe size is fixed for a 13px bar; it does not scale with the bar height
- focus box on tab labels is not done
- unfocused (backdrop) states are not specially styled

## GTK4

`gtk-4.0/` uses the same colours, gradients and measurements as the GTK3 theme, adapted to GTK4's CSS nodes
(popover menus, `entry > text`, spin buttons as one box, `menubar > item`, focus-visible outlines).
GTK4 has no scrollbar stepper buttons, so GTK4 scrollbars are the trough plus the grey grip slider only
(set `GTK_OVERLAY_SCROLLING=0` for always-visible bars). Applications built on libadwaita ignore third-party
GTK4 themes.

## GTK2

`gtk-2.0/gtkrc` is the unchanged `Clearlooks-Quicksilver` gtkrc from the original clearlooks-0.6.2 tarball. It needs a "clearlooks"
GTK2 engine installed (the engine from clearlooks 0.6.2 or the later gtk-engines).
