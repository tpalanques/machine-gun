# MachineGun virtual machine emulator

![Contributors](https://img.shields.io/github/contributors/tpalanques/machine-gun?style=plastic)
![Forks](https://img.shields.io/github/forks/tpalanques/machine-gun)
![Stars](https://img.shields.io/github/stars/tpalanques/machine-gun)
![Licence](https://img.shields.io/github/license/tpalanques/machine-gun)
![Issues](https://img.shields.io/github/issues/tpalanques/machine-gun)

## Motivation
As you may know there's plenty of published virtualization tools: VirtualBox,
VMWare, QEMU ... just to name a few. Unfortunately in my vastly ignorance and
as far as I know, all of them need chipset virtualization enabled, which is
something that I can't currently access.

And here I am, writing how MachineGun is born as a need to build a flexible
development and sand-boxing environment in a barely metal machine without
virtualization technologies enabled. Note it builds development and
sand-boxing environments, it **should not be used in production environments** as
it may have some security issues.

This project is also a way to learn some _bash_, _Docker_ and maybe some 'system
administration'. I'll try to explain things that I consider useful in an easy
way, not necessarily in a strict way. Some technologies that I use are 
really deep and won't be explained in here, if you have any questions please
refer to the proper website, I'll make my best to keep this list up to date:
+ [Apache](https://apache.org/)
+ [Bash](https://www.gnu.org/)
+ [Composer](https://getcomposer.org/)
+ [Docker](https://www.docker.com/)
+ [PHP](https://www.php.net/)
+ [MariaDB](https://mariadb.org/)

# Description
MachineGun installs docker in your machine and runs some services to build a
_web server_ system:
* An Apache server with an FPM proxy configuration
* A PHP server with some additional modules on it:
  * Composer
  * MariaDB integration
  * PDO
* A MariaDB server

# Contributions
Are more than welcome, just open an issue in
[here](https://github.com/tpalanques/machine-gun/issues/new/choose) and I'll
check it out ASAP.
