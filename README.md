Cross-dev environment has few dependencies of its own that need to be added on top of the basic junest image.
These dependencies should be easy to install in both development and integration environments.

This package will describe what these dependencies are and rely on pacman to transparently place them into
every environment.

The packages are distributed as binaries to keep the environment minimal, so anyway a custom repository have to
be configured:

```
[tools]
SigLevel = Never
Server = http://52.30.213.60:8000/tools/os/x86_64
```

Then:

```
$ pacman -Sy crossdev
```

This is ought to be simple enough to configure in any environment. The rest is done with the platform tools.
