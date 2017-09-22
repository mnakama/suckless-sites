scrollback
==========

Description
-----------

Scroll back through terminal output using Shift+{PageUp, PageDown}.

Download
--------

* [st-scrollback-0.7.diff](st-scrollback-0.7.diff)
* [st-scrollback-20170329-149c0d3.diff](st-scrollback-20170329-149c0d3.diff)

Apply the following patch on top of the previous to allow scrolling
using `Shift+MouseWheel`.

* [st-scrollback-mouse-20170427-5a10aca.diff](st-scrollback-mouse-20170427-5a10aca.diff)

Apply the following patch on top of the previous two to allow scrollback using
mouse wheel only when not in `MODE_ALTSCREEN`. For example the content is being
scrolled instead of the scrollback buffer in `less`. Consequently the Shift
modifier for scrolling is not needed anymore.  **Note: It might break other
mkeys excluding scrolling functions.**

* [st-scrollback-mouse-altscreen-20170427-5a10aca.diff](st-scrollback-mouse-altscreen-20170427-5a10aca.diff)

Notes
-----

* Patches modify config.def.h, you need to add mkeys to your own config.h
* You can not have an mshortcut for the same mkey so remove Button4 and Button5 from mshortcuts in config.h

Authors
-------

 * Jochen Sprickerhof - <st@jochen.sprickerhof.de>
 * M Farkas-Dyck - <strake888@gmail.com>
 * Ivan Tham - <pickfire@riseup.net> (mouse scrolling)
 * Ori Bernstein - <ori@eigenstate.org> (fix memory bug)
 * Matthias Schoth - <mschoth@gmail.com> (auto altscreen scrolling)
 * Laslo Hunhold - <dev@frign.de> (unscrambling, git port)
 * Paride Legovini - <pl@ninthfloor.org> (don't require the Shift modifier when using the auto altscreen scrolling)
 * Lorenzo Bracco - <devtry@riseup.net> (update base patch, use static variable for config)