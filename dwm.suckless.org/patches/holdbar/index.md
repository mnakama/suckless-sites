holdbar
=======

Description
-----------
Dwm's built-in status bar is now only shown when HOLDKEY is pressed. In addition the bar will now overlay the display. This will work regardless of the topbar setting.
This is meant to be used with the bar off by default

Notes
-----
None of the togglebar code has been removed, although you might want to remove the togglebar binding in your config.def.h.
The holdbar-modkey patch is a variant where holdbar is only active when the bar is toggled off and the holdkey can be the same the modkey.

holdbar and pertag
------------------
This version is combined with pertag patch - the state of the bar is not stored per tag - if you hide the bar on one tag, it will stay hidden on all tags. This patch applies cleanly on dwm-6.2. The holdkey is enabled by default and mapped to Mod1.


Download
--------
* [dwm-holdbar-6.2.diff](dwm-holdbar-6.2.diff)
* [dwm-holdbar-modkey-6.2.diff](dwm-holdbar-modkey-6.2.diff)
* [dwm-holdbar-modkey-pertag-nobar-6.2.diff](dwm-holdbar-modkey-pertag-nobar-6.2.diff)

Author
------
* Hayden Szymanski <hsszyman@gmail.com>
* Nihal Jere <nihal@nihaljere.xyz> (fixed flickering)
* Dariusz Fedejko <fedejko@gmail.com> (holdbar-pertag)
