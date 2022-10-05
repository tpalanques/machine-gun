# MachineGun virtual machine emulator

[//]: # (FIXME: Add license - https://github.com/tpalanques/machine-gun/issues/6)

![Contributors](https://img.shields.io/github/contributors/tpalanques/machine-gun?style=plastic)
![Downloads](https://img.shields.io/github/downloads/tpalanques/machine-gun/total)
![Forks](https://img.shields.io/github/forks/tpalanques/machine-gun)
![Stars](https://img.shields.io/github/stars/tpalanques/machine-gun)
![Issues](https://img.shields.io/github/issues/tpalanques/machine-gun)
![Closed](https://img.shields.io/github/issues-closed-raw/tpalanques/machine-gun)
![Licence](https://img.shields.io/github/license/tpalanques/machine-gun)
![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)

## 1. Motivation
As you may know there's plenty of published virtualization tools: VirtualBox,
VMWare, QEMU ... just to name a few. Unfortunately in my vastly ignorance and
as far as I know, all of them need chipset virtualization enabled, which is
something that I can't currently access.

And here I am, writing how MachineGun is born as a need to build a flexible
development and sand-boxing environment in a barely metal machine without
virtualization technologies enabled. Note it builds development and
sand-boxing environments, it **should not be used in production environments** as
it may have some security issues.

[//]: # (FIXME: Broken link - https://github.com/tpalanques/machine-gun/issues/5)

This project is also a way to learn some _bash_, _Docker_ and maybe some 'system
administration'. I'll try to explain things that I consider useful in an easy
way, not necessarily in a strict way. Some technologies that I use are 
really deep and won't be explained in here, if you have any questions please
refer to the proper website, you'll find a list of contributors in the [Credits
and contributors](#) section I'll make my best to keep this list up to date:

# 2. Description
MachineGun installs docker in your machine and runs some services to build a
_web server_ system:
* An Apache server with an FPM proxy configuration
* A PHP server with some additional modules on it:
  * Composer
  * MariaDB integration
  * PDO
* A MariaDB server

I'm using Docker because it's a trendy technology, it's well documented and
it runs without machine emulation. It does not run virtual machines but it
can be abstracted as if it were. Docker's main goal is to start services 
easily, so what we'll do is start a web sand-boxing service which is typically
hosted outside the box, this time it will be inside!

As said, I'm aware docker does not build any operating system nor machine and 
probably I'll end up by naming them machines at any point though they're 
containers, I'll do my best to be technically correct.

Also, one of the goals in this project is to keep the installer as easy as
possible, that's why I'll use strict bash, no Python, Perl or any other scripting
language will be used on top of that and packages will be kept as minimum as
it can be, this way installation will be easier.

# 3. Installation and running
By now project can't be run :(

# 4. Credits and contributions
MachineGun is possible thanks to many other lines of code. Many thanks
to all of this projects
+ [Apache](https://apache.org/)
+ [Bash](https://www.gnu.org/)
+ [Composer](https://getcomposer.org/)
+ [Docker](https://www.docker.com/)
+ [PHP](https://www.php.net/)
+ [MariaDB](https://mariadb.org/)

MachineGun is managed, developed and mantained by:
* [Toni Palanques](https://github.com/tpalanques)

Contribution are more than welcome, just open an issue in
[here](https://github.com/tpalanques/machine-gun/issues/new/choose) and I'll
check it out ASAP.
