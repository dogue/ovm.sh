+++
title = "Installation"
template = "docs/page.html"
date = "2024-02-03"
weight = 5
[extra]
toc = true
+++

## Overview

OVM lives entirely in `$HOME/.ovm` on all platforms it supports. Inside the directory, OVM will download new Odin versions and symlink whichever version you specify with `ovm use <version>` to `$HOME/.ovm/bin`. You should add this folder to your path. You should also set the environment variable `OVM_INSTALL` to the directory `$HOME/.ovm/self`. The installer should handle this for you automatically if you're on *nix systems, but you'll have to do it manually on Windows. You can then add `OVM_INSTALL` to your path.

If you don't want to use `OVM_INSTALL` (perhaps you already have OVM in a place you like), then OVM will update the exact executable that you call `upgrade` from. 

---

## Linux, BSD, MacOS, *nix

```sh
curl https://raw.githubusercontent.com/dogue/ovm/master/install.sh | bash
```

Or if you're not comfortable curl-bashing scripts from strangers on the internet, you can download it (and review it) before running.

```sh
curl https://raw.githubusercontent.com/dogue/ovm/master/install.sh -o ovm_install.sh
chmod +x ovm_install.sh
./ovm_install.sh
```

Then add OVM's directories to your `$PATH`

```
echo "# OVM" >> $HOME/.profile
echo export OVM_INSTALL="$HOME/.ovm/self" >> $HOME/.profile
echo export PATH="$PATH:$HOME/.ovm/bin" >> $HOME/.profile
echo export PATH="$PATH:$OVM_INSTALL" >> $HOME/.profile
```

---

## Windows

If you're on Windows, you can grab the [latest release](https://github.com/dogue/ovm/releases/latest)

### Putting ZVM on your Path

ZVM requires a few directories to be on your `$PATH`. If you're unfamiliar with updating environment variables on Windows, you can follow [this guide](https://www.computerhope.com/issues/ch000549.htm). Once you're in the appropriate menu, add or append to the following environment variables:

Add
* OVM_INSTALL: C:\Users\\`%YOUR_USERNAME_HERE%`\\.ovm\bin\self

Append
* PATH: C:\Users\\`%YOUR_USERNAME_HERE%`\\.ovm\bin
* PATH: $OVM_INSTALL/

---

## Arch User Repository

An AUR package for OVM is planned but not yet in place.
