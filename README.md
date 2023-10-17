# sudo-is-doas

This package was made as i use [opendoas](https://archlinux.org/packages/extra/x86_64/opendoas/) and sudo is required by some packages.

## Features

- Provides sudo
  - Pacman won't complain about sudo not being installed
- Creates a symlink from sudo to doas
  - This allows you to use doas in scripts and other programs that require sudo

## Problems

This is not a perfect solution, as doas does not provide the same interface as sudo. This means that some programs may not work with doas.

## Installation

This packages is made for Arch Linux and its derivatives - and can't be installed on other distros.

```bash
git clone https://github.com/dnorhoj/sudo-is-doas.git
cd sudo-is-doas
makepkg -si
```
