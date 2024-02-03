+++
title = "Prerequisites"
date = "2024-02-03"
template = "docs/page.html"
weight = 1
[extra]
toc = true
+++

OVM itself does not require any other software (aside from `tar` on Unix-based systems). However, due to some pecuiliarities currently affecting Odin releases, OVM builds all installs from source. This means that you need to have the required build tools and libraries installed in order to use OVM.

Unfortunately there is not a convenient list of dependencies for building Odin from source. If you run into one you're missing, please consider [creating an issue](https://github.com/dogue/ovm/issues) so that I can build a list of what is needed.

## Known dependencies

* Visual Studio (on Windows)
* LLVM (17, 14, 13, 12, or 11)
