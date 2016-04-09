Laptop
======

[![Build Status](https://travis-ci.org/camerondunford/laptop.svg?branch=master)](https://travis-ci.org/camerondunford/laptop)

Laptop is a script to set up a macOS laptop for web and mobile development.

It can be run multiple times on the same machine safely.
It installs, upgrades, or skips packages
based on what is already installed on the machine.

Requirements
------------

We support:

* macOS Mavericks (10.9)
* macOS Yosemite (10.10)
* macOS El Capitan (10.11)
* macOS Sierra (10.12)
* macOS High Sierra (10.13)
* macOS Mojave (10.14)

Older versions may work but aren't regularly tested.

Install
-------

Download the script:

```sh
curl --remote-name https://raw.githubusercontent.com/camerondunford/laptop/master/mac
```

Review the script (avoid running scripts you haven't read!):

```sh
less mac
```

Execute the downloaded script:

```sh
sh mac 2>&1 | tee ~/laptop.log
```

Optionally, review the log:

```sh
less ~/laptop.log
```

Optionally, [install camerondunford/dotfiles][dotfiles].

[dotfiles]: https://github.com/camerondunford/dotfiles#install

Debugging
---------

Your last Laptop run will be saved to `~/laptop.log`.
Read through it to see if you can debug the issue yourself.

What it sets up
---------------

macOS tools:

* [Homebrew] for managing operating system libraries.

[Homebrew]: http://brew.sh/

Unix tools:

* Bash completion
* [Git] for version control
* [GnuPG] for generating keys to sign commits
* [Zsh] as your shell

[Git]: https://git-scm.com/
[GnuPG]: https://gnupg.org/
[Zsh]: http://www.zsh.org/

Applications:

* 1Password
* Abstract
* Bartender
* Dropbox
* Firefox
* Fork
* Google Chrome
* iTerm2
* SkyFonts
* Slack
* Spotify
* Visual Studio Code
* Zoom

It should take less than 15 minutes to install (depends on your machine).


App Store
---------

* Airmail
* Magnet

License
-------

[LICENSE]

[LICENSE]: LICENSE
