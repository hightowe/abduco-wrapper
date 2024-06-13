A wrapper script to be used around abduco when the goal is to minimize
the use of the Xterm Alternate Screen Buffer, which abduco flips into
by default, both at session creation and at session attachment.

It is designed to be placed in ~/.local/bin/ or ~/bin as appropriate.

---

I use [checkinstall](https://help.ubuntu.com/community/CheckInstall) to build
a *.deb package for myself that includes this program as /usr/local/bin/abduco-wrapper.
To do that, just place this file in the abduco source/build directory, make it executable,
and add the one line to Makefile as shown in Makefile.patch.txt, and then run checkinstall.
The package that is built can then be installed and you can symlink /usr/local/bin/abduco-wrapper
to your ~/.local/bin/ or ~/bin/ directory, as appropriate.
