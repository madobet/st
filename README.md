# st - simple terminal

**st** is a simple terminal emulator for X which sucks less.


## Requirements

In order to build st you need the Xlib header files.

> **Note:**
> [This branch](https://gitlab.freedesktop.org/mawww/libxft/tree/bgra-glyphs) of libXft was used to avoid st from crashing with emoji.

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

- \[ [Alapha Focus Highlight](https://st.suckless.org/patches/alpha_focus_highlight/) \]:
  [st-alphaFocusHighlight-20191107-2b8333f.diff](https://github.com/juliusHuelsmann/st/releases/download/patchesV1/st-alphaFocusHighlight-20191107-2b8333f.diff)

- \[ [anysize](https://st.suckless.org/patches/anysize/) \]:
  [st-anysize-0.8.1.diff](https://st.suckless.org/patches/anysize/st-anysize-0.8.1.diff)
