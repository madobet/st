# st - simple terminal

**st** is a simple terminal emulator for X which sucks less.


## Requirements

In order to build st you need the Xlib header files.


## Installation

st is installed into the `/usr/local` namespace by default(if necessary as root):

    make -j clean install

You can change it by setting `PREFIX` (for example, install at `~/.local`):

    make PREFIX=~/.local -j clean install


## Running st

If you did not install st with `make clean install`, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

## Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

## Pathced with

