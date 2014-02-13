# Source Code Low

This is a fork of Adobe's [*Source Code Pro*][pro] font, with the line-height reduced
to 90% of its original value. This allows more lines of code to be displayed on a
screen while still maintaining great readability. Useful for developers who prefer
(or are forced) to work with smaller windows/screens.

> Source Code Pro is a set of OpenType fonts that have been designed to work well
> in user interface (UI) environments. In addition to a functional OpenType font, this open
> source project provides all of the source files that were used to build this OpenType font
> by using the AFDKO makeotf tool.

[pro]: https://github.com/adobe/source-code-pro


## Building from source

### Requirements

To build the binary font files from source, you need to have installed the
[Adobe Font Development Kit for OpenType](http://www.adobe.com/devnet/opentype/afdko.html) (AFDKO). The AFDKO
tools are widely used for font development today, and are part of most font
editor applications.

### Building one font

The key to building OTF or TTF fonts is `makeotf`, which is part of the AFDKO toolset.  
Information and usage instructions can be found by executing `makeotf -h`.

In this repository, all necessary files are in place for building the OTF and TTF fonts.  
For example, build a binary OTF font for the Regular style like this:

```sh
$ cd Roman/Regular/
$ makeotf -r
```

### Building all fonts

For convenience, a shell script named `build.sh` is provided in the root directory.  
It builds all OTFs and TTFs, and can be executed by typing:

```sh
$ ./build.sh
```

