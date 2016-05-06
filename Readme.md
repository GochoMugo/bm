## BM

>  Simple bash CLI bookmarks with tag support<br>
>  This is a fork that removes everything unneccessary.<br>
>  Like DropBox, Previews.<br>
>  Also modified default behavior,<br>
>  replaced description with date field.<br>
>  &mdash; by [@noqqe](https://github.com/noqqe)
>
>  Kind of Simplified the help information.<br>
>  Added the `help` and `version` commands.<br>
>  Allow changing the default `$PREFIX` during install.<br>
>  Use `grep` instead of `ggrep`, for Linux<br>
>  &mdash; by [@GochoMugo](https://github.com/GochoMugo)


## Install

```bash
$ make install
$ make uninstall
```

**Note**: you can use `$PREFIX` to change installation location,
as usual, e.g. `PREFIX=~ make install`


## Example

  Add a bookmark:

    $ bm add http://subtlepatterns.com design textures

  Search for a bookmark:

    $ bm search noqqe

## Usage

```

Usage: bm [cmd]

  Commands:

    # add a bookmark with the given url and optional tags
    $ bm add <url> [tag...]

    # list bookmarks available
    $ bm list|ls
    $ bm
    $ bm 20

    # open the first bookmark matching <query>
    $ bm open <query>

    # search the bookmarks via full-text <query>
    $ bm search <query>

    # list tags
    $ bm tags

    # display statistics about the bookmarks
    $ bm statistics
    $ bm stats

    # show help information
    $ bm help|-h|--help

    # show version information
    $ bm version|-V|--version

```

## File Stucture

```
$ cat ~/.bookmarks
http://vimeo.com/6200166|bike fixie|2014-08-06T07:36:56Z|One gear No idea on Vimeo
http://z0r.de/?id=38|Fun|2010-01-24T19:25:36Z|ZOMG ZUFALL! #38
```
