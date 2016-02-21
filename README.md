[![Documentation](https://readthedocs.org/projects/restic/badge/?version=latest)](https://restic.readthedocs.org/en/latest/?badge=latest)
[![Build Status](https://travis-ci.org/restic/restic.svg?branch=master)](https://travis-ci.org/restic/restic)
[![Build status](https://ci.appveyor.com/api/projects/status/nuy4lfbgfbytw92q/branch/master?svg=true)](https://ci.appveyor.com/project/fd0/restic/branch/master)
[![Report Card](http://goreportcard.com/badge/restic/restic)](http://goreportcard.com/report/restic/restic)
[![Coverage Status](https://coveralls.io/repos/restic/restic/badge.svg)](https://coveralls.io/r/restic/restic)


Introduction
============

restic is a backup program that is fast, efficient and secure. Detailed
information can be found in [the documentation](doc/index.md) and [the user
manual](doc/Manual.md). The [design document](doc/Design.md) lists the
technical background and gives detailed information about the structure of the
repository and the data saved therein.

The latest documentation can be viewed online at
<https://restic.readthedocs.org/en/latest>. On the bottom left corner there is
a menu that allows switching to the documentation and user manual for the
latest released version.

Build restic
============

Install Go/Golang (at least version 1.3), then run `go run build.go`,
afterwards you'll find the binary in the current directory:

    $ go run build.go

    $ ./restic --help
    Usage:
      restic [OPTIONS] <command>
    [...]

More documentation can be found in the [user manual](doc/Manual.md).

At the moment, the only tested compiler for restic is the official Go compiler.
Building restic with gccgo may work, but is not supported.

Contribute and Documentation
============================

Contributions are welcome! More information can be found in
[`CONTRIBUTING.md`](CONTRIBUTING.md). A document describing the design of
restic and the data structures stored on the back end is contained in
[`doc/Design.md`](doc/Design.md).
The development environment is described in [`CONTRIBUTING.md`](CONTRIBUTING.md).

Contact
=======

If you discover a bug, find something surprising or if you would like to
discuss or ask something, please [open a github issue](https://github.com/restic/restic/issues/new).
If you would like to chat about restic, there is also the IRC channel #restic
on irc.freenode.net.

**Important**: If you discover something that you believe to be a possible critical
security problem, please do *not* open a GitHub issue but send an email directly to
alexander@bumpern.de. If possible, please encrypt your email using the following PGP key
([0x91A6868BD3F7A907](https://pgp.mit.edu/pks/lookup?op=get&search=0xCF8F18F2844575973F79D4E191A6868BD3F7A907)):

```
pub   4096R/91A6868BD3F7A907 2014-11-01
      Key fingerprint = CF8F 18F2 8445 7597 3F79  D4E1 91A6 868B D3F7 A907
      uid                          Alexander Neumann <alexander@bumpern.de>
      uid                          Alexander Neumann <alexander@debian.org>
      sub   4096R/D5FC2ACF4043FDF1 2014-11-01
```

License
=======

Restic is licensed under "BSD 2-Clause License". You can find the complete text
in the file `LICENSE`.
