Collection of SyzKaller reproducers for issues linked to MPTCP
==============================================================

This repository contains reproducers for issues linked to MPTCP. It is designed
to be used by a CI to look for regressions.

Structure
---------

The structure is then important for developers to quickly find from where the
issues came from originally. It is also important for the CI to know what to
use.

Current structure:
* Issues reported on Github can be added in the `github` directory, e.g.:
  `upstream/github/issues/<closed|opened>/<id>`
* In this directory, you can add C files, kernel config, syzkaller reproducer
  files and text file containing additional info, e.g.
```
├── <name>.c
├── <name>.kconfig
├── <name>.syzkaller
└── <name>.info
```
