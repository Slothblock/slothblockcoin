
Debian
====================
This directory contains files used to package slothblockcoind/slothblockcoin-qt
for Debian-based Linux systems. If you compile slothblockcoind/slothblockcoin-qt yourself, there are some useful files here.

## slothblockcoin: URI support ##


slothblockcoin-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install slothblockcoin-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your slothblockcoin-qt binary to `/usr/bin`
and the `../../share/pixmaps/slothblockcoin128.png` to `/usr/share/pixmaps`

slothblockcoin-qt.protocol (KDE)

