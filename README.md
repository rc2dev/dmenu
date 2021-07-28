# dmenu - dynamic menu

Build of dmenu by [Rafael Cavalcanti](https://rafaelc.org).

dmenu is an efficient dynamic menu for X.

## Third party patches

- case-insensitive
- grid
- gridnav
- highlight
- line-height
- password

## My own patches

- Remove empty lines dynamically.
- Make movements more vim-like and use Ctrl instead of Alt.
  `Ctrl+jklh` work as you would expect, be it on horizontal list, vertical list or grid.
- Use ctrl+v/V instead of ctrl+y/Y.
- Move colors to separate file. Add file with default colors.
- Complement to `case-insensitive` patch: Keep a dummy `-i` option, so 3rd party scripts don't fail.
- Complement to `hightlight`patch: Add CLI options for highlight colors.

## Requirements

In order to build dmenu you need the Xlib header files.

## Installation

Edit config.mk to match your local setup (dmenu is installed into the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu (if necessary as root):

```sh
make clean install
```

## Running dmenu

See the man page for details.
