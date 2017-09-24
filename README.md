grep-locate
===========

Faster, user-space oriented locate and updatedb.
System wide usage as root may expose "hidden" files.
For system wide, make sure to set XDG_DATA_HOME to some meaningful
location.

Ignoring Directories
---------------------

To ignore certain directories, you can set a global /etc/updatedb-ignore
which contains full paths to directories; they must not be files.
the user can also use \$XDG_CONFIG_HOME/updatedb-ignore or
\$HOME/.config/updatedb-ignore to accomplish the same thing.
