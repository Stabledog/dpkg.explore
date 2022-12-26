# dpkg.explore

## BB DPKG

### Materials and links
- Training material dpkg:  https://bbgithub.dev.bloomberg.com/pages/training-materials/dpkg/
- Also ELRN video series
- Devx dpkg portal:  https://dpkg.dx.bloomberg.com/


## Public Debian world
[Debian guide for maintainers](https://www.debian.org/doc/manuals/debmake-doc/index.en.html)
[Bloomberg dpkg portal](https://dpkg.dx.bloomberg.com/)
[Daniel Persson tutorial video](https://www.youtube.com/watch?v=-QrvP1m7ReI&ab_channel=DanielPersson)

## Setup
- Install `dpkg-dev` `devscripts`
- Install `debmake` and `debmake-doc` for public dpkg guide
- Install `quilt`
- Install `debaid` shellkit
- Install ~/.taskrc/dpkg.taskrc
- Install `sbuild` as described in $3.6 of the "Debian guide for maintainers"


## Plan
- dbash Let's make an update to `bash` that applies a trivial patch, in anticipation of adding debug hooks

## Commands

- Get source:
    ```
    apt-get source [packagename] # Extract source into ./
    ```
    This depends on having enabled/uncommented the `deb-src` rows in /etc/apt/sources.list, and possibly doing an `apt-get update` to sync cache first.


## Notes
- /var/log/dpkg.log shows dpkg activity
- /etc/dpkg/ << machine config
- The `reprepro` package is used to set up your own package repo
- Shellkit has `debaid` to help with dpkg tasks
