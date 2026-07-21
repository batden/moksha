# Moksha Desktop

![Moksha Desktop](https://www.enlightenment.org/ss/e-6a5fbe7558b1b1.59929539.png)  

**A fast, lightweight, and highly customizable desktop environment** — a modern community fork of Enlightenment DR17.

Moksha is the default desktop of **[Bodhi Linux](https://www.bodhilinux.com/)** and focuses on **speed, stability, and flexibility** while staying true to the lightweight philosophy of its predecessor.

## Why Moksha?

- Extremely lightweight and fast — runs great on old and new hardware
- Highly customizable with beautiful maintained themes
- Excellent keyboard-driven workflow
- Useful extra moksha modules
- Clean, bloat-free user experience

## Key Features

- Advanced theming system using Edje
- Modular architecture - easy to extend
- Backward compatible with many E17/E18 modules and themes
- Compositing possible with Picom module

## Installation

Requirements:
-------------
Autoconf version 2.71 is now required.

Dependencies for building under Bodhi:
  doxygen pkg-config libglib2.0-dev libssl-dev libpng12-dev libharfbuzz-dev
  libfribidi-dev libfontconfig1-dev libluajit-5.1-dev libsndfile1-dev
  libpulse-dev libbullet-dev libxcb1-dev libxcb-shape0-dev libxcb-keysyms1-dev
  automake libx11-xcb-dev libudisks2-dev

Must:
  libc libm libX11 libXext evas ecore ecore-evas ecore-file ecore-ipc ecore-con
  ecore-imf ecore-x edje eet embryo efreet eldbus eio
  xcb xcb-shape xcb-keysyms

You can also use the configure --prefix option to put Moksha in a separate tree
of its own (recommended) like:

./autogen.sh --prefix=/usr/local/moksha


### Build from Source

```bash
git clone https://github.com/JeffHoogland/moksha.git
cd moksha
./autogen.sh --prefix=/usr
make
sudo make install
