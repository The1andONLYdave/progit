progit
======

German Version of Progit Ebook (https://github.com/progit/progit) ready to use. Creative Commons Attribution-Non Commercial-Share Alike 3.0 license

Binary Compiled files for reading. Wanted to download a german version but didn't find any and couldn't build on my PC at work, so here they are. Any more formats please send me a mail. New Versions too.

Fertige Ausgaben des Progit Buches auf Deutsch. Ich habe keine deutsche Version im Netz gefunden und kann es auf der Arbeit am PC nicht bauen, deswegen hier zum download. Wenn du weitere Formate oder neue Versionen möchtest mail mir.

------------progit readme follow------------
[![Build Status](https://secure.travis-ci.org/progit/progit.png?branch=master)](https://travis-ci.org/progit/progit)

# Pro Git Book Contents

This is the source code for the Pro Git book contents.  It is licensed under
the Creative Commons Attribution-Non Commercial-Share Alike 3.0 license.  I
hope you enjoy it, I hope it helps you learn Git, and I hope you'll support
Apress and me by purchasing a print copy of the book at Amazon:

http://tinyurl.com/amazonprogit

It is also available online at:

http://git-scm.com/book/

and fully translated in 10 languages.

# Making Ebooks

On Fedora (16 and later) you can run something like this::

    $ yum install ruby calibre rubygems ruby-devel rubygem-ruby-debug rubygem-rdiscount
    $ makeebooks en  # will produce a mobi

On MacOS you can do like this::
	
1. INSTALL ruby and rubygems
2. `$ gem install rdiscount`
3. DOWNLOAD Calibre for MacOS and install command line tools. You'll need some dependencies to generate a PDF:
    * pandoc: http://johnmacfarlane.net/pandoc/installing.html
    * xelatex: http://tug.org/mactex/
4. `$ makeebooks zh` #will produce a mobi

## Notes on pandoc

Please use Pandoc version 1.11.1 or later as older versions(confirmed on 1.9.1.1) has a [bug](https://github.com/jgm/pandoc/issues/964) which hides a word after tilde `~`.  You can do `pandoc -v` to see which version you have installed.

# Errata

If you see anything that is technically wrong or otherwise in need of
correction, please [open an issue](https://github.com/progit/progit/issues/new) and one of the maintainers will take a look.


# Translation

If you wish to translate the book, your work will be put up on the 
git-scm.com site.  Please put your translation into the appropriate
subdirectory of this project, using the 
[ISO 639](http://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) 
and send a pull request.

# Sending a pull request

* Be careful to use UTF-8 encoding in your files.
* Do not mix changes to the original english with translations in a single pull request.
* If your pull request changes a translation, prefix your pull request and commits'messages with the ISO 639 code, e.g. `[de] Update chapter 2`. Please only push files where there is already some translation done.
* Make sure the translation changes can be automatically merged. The maintainers can not make the merge manually if there are some conflicts.
* Make as sure as possible that the changes work correctly for publishing to pdf, ebooks and the git-scm.com website
