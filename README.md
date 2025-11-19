# Adwaita

Building blocks for modern GNOME applications.

## About this fork

This is a fork of libadwaita designd to fit in better with KDE 

it's going to have a more UWP (WinUI) like appearance to fit in with the modern aesthetic of KDE

all done without breaking ABI compatibility at all so there's no need to recompile

Current official targets:

Fedora 43 (amd64)

Almalinux 10 (aarch64, x86-64-v2)

Feel free to package this for you KDE based distributions (base doesn't matter)

## License

Libadwaita is licensed under the LGPL-2.1+.

## Building

We use the Meson (and thereby Ninja) build system for libadwaita. The quickest
way to get going is to do the following:

```sh
meson setup _build
ninja -C _build
ninja -C _build install
```

For build options see [meson_options.txt](./meson_options.txt). E.g. to enable documentation:

```sh
meson setup _build -Ddocumentation=true
ninja -C _build
```

## Usage

There's a C example:

```sh
_build/run _build/demo/adwaita-1-demo
```

## Documentation

The documentation can be found online
[here](https://gnome.pages.gitlab.gnome.org/libadwaita/doc/).

## Getting in Touch

Matrix room: [#libadwaita:gnome.org](https://matrix.to/#/#libadwaita:gnome.org)

