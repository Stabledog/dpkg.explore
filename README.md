# dpkg.explore

[Debian guide for maintainers](https://www.debian.org/doc/manuals/debmake-doc/index.en.html)
[Bloomberg dpkg portal](https://dpkg.dx.bloomberg.com/)

## Setup
- Install `debmake` and `debmake-doc` for public dpkg guide
- Install `quilt`
- Install `debaid` shellkit
- Install ~/.taskrc/dpkg.taskrc
- Install `sbuild` as described in $3.6 of the "Debian guide for maintainers"


## Commands

- Get source:
    ```
    apt-get source [packagename] # Extract source into ./
    ```
    This depends on having enabled/uncommented the `deb-src` rows in /etc/apt/sources.list, and possibly doing an `apt-get update` to sync cache first.


## Notes
/var/log/dpkg.log shows dpkg activity
/etc/dpkg/ << machine config
