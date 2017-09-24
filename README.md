grep-locate
===========
Faster, user-space oriented locate and updatedb.

Running as Root
---------------

System wide usage as root may expose "hidden" files.
When run as root the db will be written to /var/lib/glocate/glocate.db
if users don't have their own db, they will use this one.

Ignoring Directories
---------------------

To ignore certain dirs, you can set a global /etc/updatedb-ignore
which contains find style path patterns to directories.
the user can also use $XDG_CONFIG_HOME/updatedb-ignore or
$HOME/.config/updatedb-ignore to accomplish the same thing.

### Examples

Ignore all .git directories:

    */.git

Ignore a particular user's folder:

    /home/username

See the manpage for your `find` command for details about the -path option and the pattern it takes.
