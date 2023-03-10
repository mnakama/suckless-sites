dynamic options
================

Description
-----------
This patch adds a flag (`-dy`) which makes dmenu run the command given to it
whenever input is changed with the current input as the last argument and
update the option list according to the output of that command.

By default dmenu does not let you change the option list after starting it,
this patch adds support for that.
It is best used with the -l flag.

(ie. usage: `dmenu -dy ls` runs ls on whatever directory/file you are currently typing
in dmenu and lets you select it)

Download
--------
* [dmenu-dynamicoptions-5.0.diff](dmenu-dynamicoptions-5.0.diff) (with proper command quoting)
* [dmenu-dynamicoptions-20200526-01e2dfc7.diff](dmenu-dynamicoptions-20200526-01e2dfc7.diff) (2020-05-26)

Author
------
* ttmx - tiago.sequeira.teles@gmail.com (2020-05-26)
* Ziad EL KHOURY HANNA - me@ziadkh.ovh (5.0)
