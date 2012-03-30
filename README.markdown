From Miek Giebn's [original blog post](http://www.miek.nl/s/d7c7a15ac3/ "Blockbook.cls; A LaTeX Class"):

### LaTeX Style ###
A few years ago I've created a LaTeX class which I particularly liked, but looking back on it, it was getting a bit old. So I recreated they style with the excellent `memoir` class for LaTeX.

#### Class File ####
The style consists out of a single class file, called blocksbook.cls. Just put it somewhere, where TeX can find it (i.e. the current directory) and use it with: `\documentclass{blocksbook}`.

All options from `memoir` are supported in addition to:

* `draft` - puts the word 'draft' in the header, also given to `memoir`
* `serif` - use the 'serif' font
* `headbold` - use the bold font in the headings
* `bold` - use bold font in itemize
* `bottomline` - draw a `\hrule` under each page, excluding part and chapter pages.
* `titlepagenr` - show a blocked page number on the title page.

---

### Places Used ###
Blocksbook is currently used by [Miek's introduction to Go](https://github.com/miekg/gobook).

### Latest Changes ###
* Fix the title page - a blocked page number is optionally printed.
* Per default, don't draw an `\hrule` (see option `bottomline`).
* Number subsection also
* Some spacing issues are fixed