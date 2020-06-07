# dwm-patches
Patches for dwm that I've edited or created.
dwm-systray_toggle applies on top of [dwm-systray](https://dwm.suckless.org/patches/systray/) and is also available there.
dwm-statuscolors-statuscmd-signal-6.2.diff is a combination of [dwm-statuscolors](https://dwm.suckless.org/patches/statuscolors/)
and [dwm-statuscmd-signal](https://dwm.suckless.org/patches/statuscmd/). The issue with these patches was, that they
used the same range of escape characters to achieve completely different things. This patch splits the range of characters at
roughly 16 each, theoretically allowing 16 dwmblocks modules that can be signalled and 16 color
schemes for the status bar, which should be plenty. An alternative would be to use a different kind of sequence for the color
patch and rewrite it accordingly (which I might do just for the heck of it...)
