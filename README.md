# scripts
Archlinux scripts

**************************************************************************************
ARCHLINUX ULTIMATE INSTALL (https://github.com/helmuthdu/aui)
Increase cowspace partition:

mount -o remount,size=2G /run/archiso/cowspace

install git:

pacman -Sy git

get the script:

git clone git://github.com/helmuthdu/aui

cd aui && ./fifo

riavviare e, dal sistema operativo appena installato (ovviamente parte da console), loggarsi come root e:

cd aui && ./lilo

ATTENZIONE!!!
la scelta della localizzazione italiana della tastiera (select keymap) è 111
la scelta del locale (select locale) è 158

**************************************************************************************
ARCH LINUX FAST INSTALLER (https://github.com/MatMoul/archfi)
Download the script with from the command line:

curl -L archfi.sf.net/archfi > archfi

or:

curl -L matmoul.github.io/archfi > archfi

launch the script:

sh archfi

**************************************************************************************
ATTENZIONE!!!
Arch User Repository
Install a pacman wrapper for AUR support, for example trizen, yay,ecc.:

$ sudo pacman -S git
$ cd /tmp
$ git clone https://aur.archlinux.org/trizen.git
$ cd trizen
$ makepkg -si
