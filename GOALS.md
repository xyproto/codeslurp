## The dream

* No more `/usr/local/src`!
* Have an open source system where all the sources for everything on the system is in a single place!
* Format spaces and tabs in all the source code on all of your system to your liking! ;)
* Perform security fixes to C code to all source code on your system.
* Automatic building and installation of executables and libraries as the source database changes, once the new source compiles and functional tests looks good.
* Upgrade packages only by upgrading source code. This is where the upgrade process belongs.
* Provide compiler wrappers that fetches source code from the database on demand.
* Share the database of a working system with others.
* Easy for upstream to pick up popular (working) improvements to the source code.
* Easy for IDEs to provide ways to navigate and debug all the source code on the system.
* As long as functional tests + GUI tests are in place, the things you care about will always keep working.

## Other ideas

* A new project `flagslurp` for storing a per-file CFLAGS / CXXFLAGS / configure / CMake list of flags, with inheritance of flags from either the parent directory, a specific directory or one of the system-wide flag collections.
* A new project `systemslurp` for storing per-system hardware configuration.
* A new project `userslurp` for storing per-user configuration, with a username/password for storing all user preferences, like: themes, timezone, keyboard layout, favorite editor, favorite browser, favorite filesystem partition layout and partition formatting flags.
* Combined, it should be everything a Linux distro needs: `source code + compile flags + system config + user config`
