# steghide

This is a copy of the original [steghide](http://steghide.sourceforge.net/) sources (v0.5.1).
The sources are modified to compile on macOS Monterey (12.4) and probably earlier and later versions.

You need libmhash and libmcrypt to compile. If you're using Homebrew as package manager, just type

```
brew install mhash mcrypt
```

to install the libraries.

Then, after cloning this repository with

```
git clone https://github.com/raetselonkel/steghide.git
```

you may enter the the folder and build `steghide`:

```
cd steghide
./configure
make
```

Don't panic, when the build fails while executing `libtool`. Just type

```
./postmake.sh
```

and, voilà!, `steghide` will be generated in the folder src.
