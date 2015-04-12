## BM

  Simple bash CLI bookmarks with tag support
  This is a fork that removes everything unneccessary.
  Like DropBox, Previews.

  Also modified default behavior, replaced description with date field.


## Install

```
$ make install
$ make uninstall
```

## Example

  Add a bookmark:

    $ bm add http://subtlepatterns.com design textures

  Search for a bookmark:

    $ bm search noqqe

## Usage

```

Usage: bm [options] [cmd]

Commands:

  # add a bookmark with the given url and optional tags
  $ bm add <url> [tag...]

  # open the first bookmark matching <query>
  $ bm open <query>
  $ bm <query>

  # search the bookmarks via full-text <query>
  $ bm search <query>

  # list bookmarks available
  $ bm list
  $ bm ls
  $ bm

Options:

   -V, --version   output bm version
   -h, --help      output this help information

```

## File Stucture

```
$ cat ~/.bookmarks
http://vimeo.com/6200166|bike fixie|2014-08-06T07:36:56Z|One gear No idea on Vimeo
http://z0r.de/?id=38|Fun|2010-01-24T19:25:36Z|ZOMG ZUFALL! #38
```

## Pitfalls

* I use `bm` on OpenBSD. If you're on Linux you may have to replace `ggrep`
  with `grep`
