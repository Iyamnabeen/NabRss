NabRss [ NABEEN'S minimal RSS feed reader ]
======
Installation
------------
Run this command to build NabRss:

	make clean install

This will install the binary to ~/.local/bin. Make sure that this directory is
in your $PATH.

If you need to change this, set the PREFIX variable in Makefile.

Configuration
-------------
NabRss is configured via the config.h file, which you can create by
either compiling MinRSS for the first time or copying config.def.h
to it. To save your changes, recompile NabRss

Using NabRss
------------
Make a directory to store your RSS feeds, then cd into it. Then, enter 
the minsrss command to download the RSS feeds. Your feeds will be 
available as folders in your current working directory.

Compatibility
-------------
This program is designed to work on Linux, but it should be possible
to make it run on other operating systems. If you can do that
successfully, please contact me about it.

Note that if you use MinRSS on different systems, it will be possible for
attackers to write malicious filenames, so you should rewrite sanitize()
accordingly.
