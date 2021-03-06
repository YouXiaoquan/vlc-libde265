# vlc-libde265

Plugin for VLC 2.x to support HEVC decoding using libde265. For VLC
versions below 2.1, a modified MKV demuxer is included which has support
for HEVC streams. For VLC versions below 2.2, a modified MPEG-TS demuxer
is included which has support for HEVC streams.


## Building

[![Build Status](https://travis-ci.org/strukturag/vlc-libde265.png?branch=master)](https://travis-ci.org/strukturag/vlc-libde265)

Execute the default `configure` / `make` steps:

    $ ./configure
    $ make

If you fetched vlc-libde265 from GitHub, you will need to generate the
`configure` script first:

    $ ./autogen.sh


## Dependencies

In addition to a compiler, a couple of other packages must be installed
in order to compile the plugin:
- libvlccore-dev
- libde265-dev (>= 0.7)
- libebml-dev
- libmatroska-dev
- libdvbpsi-dev

These should be available from the package management on any recent
version of Debian / Ubuntu.


## Patches

See the `patches` folder for changes applied to the VLC source code of
the MKV and MPEG-TS demuxer to make it compile against older versions of
VLC in this plugin.


## Packages

Binary packages for Ubuntu are available on Launchpad:
https://launchpad.net/~strukturag/+archive/libde265


Copyright (c) 2014 struktur AG
