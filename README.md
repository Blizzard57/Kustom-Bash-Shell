# Kustom Shell

## General

The code was tested out with Ubuntu 20.04 running on WSL2, thus hardware interrupts were not tested extensively. The newborn command does not work but the idea behind the command is given in the code (stack smashing occurs). Also all process related details are taken from /proc virtual filesystem and thus does not work on other operating systems.

## Main Shell

The shell allows I/O redirection, Piping, Process Management and Signal Handling. It sets up the current dirctory as the home dircetory and allows `cd` to send it back to home. It also allows usage of `~` for indicating the home folder.