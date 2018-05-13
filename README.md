# linux-commands

Check all running daemons in linux
$ ps -eo 'tty,pid,comm' | grep ^?

If root is running graphical programs, they will show up.
Daemons running without root privileges won't. Note that daemons which start at boot time are usually running as root.

$ ps -U0 -o 'tty,pid,comm' | grep ^?
