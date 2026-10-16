# Theme details, credits and licences

## Details
| Folder (in `themes/`) | Based on | GTK2 | GTK3 | GTK4 | Xfwm4 |
|---|---|---|---|---|---|
| Clearlooks | gtk-engines 2.20.2 Clearlooks | original | ported | ported | recoloured |
| Clearlooks-classic | clearlooks-0.6.2 Clearlooks | original | ported | ported | recoloured |
| Clearlooks-classic-deepsky | clearlooks-0.6.2 DeepSky | original | ported | ported | recoloured |
| Clearlooks-classic-olive | clearlooks-0.6.2 Olive | original | ported | ported | recoloured |
| Clearlooks-classic-quicksilver | clearlooks-0.6.2 Quicksilver | original | ported | ported | recoloured |
| Crux | gtk-engines 2.20.2 Crux | original | ported | ported | recoloured |
| Cruxblu | gtk-engines 2.20.2 Crux | modified | ported | ported | original Crux |
| Industrial | gtk-engines 2.20.2 Industrial | original | ported | ported | modified |
| Mist | gtk-engines 2.20.2 Mist | original | ported | ported | new |
| Redmond | gtk-engines 2.20.2 Redmond | original | ported | ported | original |
| Redmond-aspen | gtk-engines 2.20.2 Redmond, dark colours after Greybird-dark | modified | ported | ported | modified |
| ThinIce | gtk-engines 2.20.2 ThinIce | original | ported | ported | new |

## Credits
These themes are CSS ports of the GTK2 themes and engines below. All of the design and the original code
belong to their authors; the GTK3/GTK4 ports were written entirely by Claude (Anthropic), by building
from the engine source and comparing the result pixel by pixel with real GTK2 renderings.

| Theme | Original work |
|---|---|
| Clearlooks | gtk-engines 2.20.2 Clearlooks: Richard Stellingwerff, Daniel Borgmann, Benjamin Berg, Andrea Cimitan (and the contributors in the engine's CREDITS) |
| Clearlooks-classic, -deepsky, -olive, -quicksilver | clearlooks 0.6.2 and its themes: Richard Stellingwerff, Daniel Borgmann; based on Bluecurve (Red Hat; Garrett LeSage, Alexander Larsson). Colour schemes by Billy Cantrell, Marc Schwartz, JP Bizet and others |
| Industrial | gtk-engines 2.20.2 Industrial: designed by Tigert and Jimmac, implemented by Christopher James Lahey; based on the Bluecurve theme (Garrett LeSage, Alexander Larsson) and the Metal theme (Randy Gordon, Owen Taylor); Cairo port by Benjamin Berg |
| Redmond | gtk-engines 2.20.2 Redmond: Owen Taylor (original Redmond95), Andrew Johnson (cleanup and revisions) |
| Mist | gtk-engines 2.20.2 Mist: Dave Camp (Ximian), loosely based on ThinIce |
| ThinIce | gtk-engines 2.20.2 ThinIce: Tim Gerla, Tomas Ögren, Richard Hult |
| Crux | gtk-engines 2.20.2 Crux: Arlo Rose (design), John Harper (implementation), Seth Nickell (GTK2 implementation), Josh Barrow (original GTK+ theme); Lapo Calamandrei and Thomas Wood for the later gtkrc |

The Xfwm4 themes are based on the Xfwm4 themes of Casey Kirsle (Clearlooks, via [Clearlooks-Phenix](https://github.com/jpfleury/clearlooks-phenix)), Erçin Eker (Industrial) and xfwm4-themes (Crux, Redmond, Redmond-aspen). The dark colours of Redmond-aspen are taken from Greybird-dark.

## Licences
The ports are derived from existing GPL/LGPL code, so they carry the same licences:

- Clearlooks, Industrial, Redmond, Mist, ThinIce, Crux, Cruxblu (derived from gtk-engines 2.20.2): GNU LGPL 2.1 or later, see [LGPL-2.1](./LICENSE).
- Clearlooks-classic and its variants deepsky, olive, quicksilver (derived from clearlooks 0.6.2): GNU GPL 2 or later, see [GPL-2](./COPYING-GPL-2).

The `gtk-2.0` folders hold the unchanged gtkrc files of the original themes.

### Xfwm4 themes
- Mist and ThinIce (drawn for this project to match the GTK themes): GNU LGPL 2.1 or later, like the GTK ports.
- Industrial: based on the Ximian Desktop 2 default window decoration by Erçin Eker (GPL).
- Clearlooks and the Clearlooks-classic variants: recolours of the Clearlooks Xfwm4 theme by Casey Kirsle, taken from [Clearlooks-Phenix](https://github.com/jpfleury/clearlooks-phenix), which lists it under the GPL (version not stated).
- Crux, Cruxblu and Redmond: from xfwm4-themes (GPL 2 or later). Crux is a port of the Sawfish theme of the same name; Redmond is a port of the Oroborus theme "windows".
