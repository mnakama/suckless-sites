search engines
==============

Description
-----------

This patch allows the simple use of search engines. Put something
like this in your `config.h`:

	static SearchEngine searchengines[] = {
		{ "g ",   "http://www.google.de/search?q=%s"   },
		{ "leo ", "http://dict.leo.org/ende?search=%s" },
	};

Then you can access each search engine by putting its prefix in front of your 
keywords:

	g foo bar

or:

	leo hello

**Note:** tokens should end with a space to prevent matching when trying to
search for a url. Token `"g"` will match `google.com`.

Using `" "` as your token will give you the functionality of the
[spacesearch](https://surf.suckless.org/patches/spacesearch/) patch.

Download
--------

* [surf-0.3-searchengines.diff](surf-0.3-searchengines.diff) (2107) (20091204)
* [surf-0.4-searchengines.diff](surf-0.4-searchengines.diff) (2107) (20091204)
* [surf-0.7-searchengines.diff](surf-0.7-searchengines.diff) (20151219)
* [surf-git-20160127-searchengines.diff](surf-git-20160127-searchengines.diff)
* [surf-0.7-webkit2-searchengines.diff](surf-0.7-webkit2-searchengines.diff) (20160108)
* [surf-git-20170323-webkit2-searchengines.diff](surf-git-20170323-webkit2-searchengines.diff)
* [surf-searchengines-20220804-609ea1c.diff](surf-searchengines-20220804-609ea1c.diff)

Author
------

* Nils Schweinsberg (McManiaC) <mail@n-sch.de>
* Samuel Baldwin (shardz) <recursive.forest@gmail.com>
* Alex Puterbaugh (zombine) <puterbaugh0@gmail.com>
* Ivan Tham (pickfire) <pickfire@riseup.net>
* Juan Aguilar Santillana (botika) <aritmeeul@gmail.com>
* Justinas Grigas - <jstn_as@protonmail.com> (20220804 version)
