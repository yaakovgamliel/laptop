Laptop
======

Laptop is a script to set up an OS X laptop for iOS development.

It can be run multiple times on the same machine safely.
It installs, upgrades, or skips packages
based on what is already installed on the machine.

Note
====
This is a fork and  We’ve change the script to only install the packages listed here.

Requirements
------------

We support:

* [OS X Mavericks (10.9)](https://itunes.apple.com/us/app/os-x-mavericks/id675248567)
* [OS X Yosemite (10.10)](https://www.apple.com/osx/)

Older versions may work but aren't regularly tested. Bug reports for older
versions are welcome.

Install
-------

Download, review, then execute the script:

```sh
curl --remote-name https://raw.githubusercontent.com/yaakovgamliel/laptop/master/mac
less mac
sh mac 2>&1 | tee ~/laptop.log
```

What it sets up
---------------
* [Homebrew] for managing operating system libraries
* [Mogenarator] for managing Core Data stuff
* [ImageMagick] for cropping and resizing images
* [Ghostsript] for making cute little version numbers in the app’s icon

[Homebrew]: http://brew.sh/
[ImageMagick]: http://www.imagemagick.org/
[Mogenerator]: http://rentzsch.github.io/mogenerator/
[Ghostscript]: http://www.ghostscript.com
It should take less than 5 minutes to install (depends on your machine).



Credits
-------

![thoughtbot](http://thoughtbot.com/assets/tm/logo.png)

Laptop is maintained and funded by [thoughtbot, inc](http://thoughtbot.com/community).
The names and logos for thoughtbot are trademarks of thoughtbot, inc.

Thank you, [contributors](https://github.com/thoughtbot/laptop/graphs/contributors)!

Contributing
------------

Edit the `mac` file.
Document in the `README.md` file.
Follow shell style guidelines by using [ShellCheck] and [Syntastic].

```sh
brew install shellcheck
```

[ShellCheck]: http://www.shellcheck.net/about.html
[Syntastic]: https://github.com/scrooloose/syntastic

License
-------

Laptop is © 2011-2014 thoughtbot, inc. It is free software, and may be
redistributed under the terms specified in the LICENSE file.
