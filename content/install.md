+++
title = "Installing OVM"
+++

OVM lives entirely in `$HOME/.ovm` on all platforms it supports. Inside the directory, OVM will download new Odin versions and symlink whichever version you specify with `ovm use <version>` to `$HOME/.ovm/bin`. You should add this folder to your path. You should also set the environment variable `OVM_INSTALL` to the directory `$HOME/.ovm/self`. The installer should handle this for you automatically if you're on *nix systems, but you'll have to do it manually on Windows. You can then add `OVM_INSTALL` to your path.

If you don't want to use `OVM_INSTALL` (perhaps you already have OVM in a place you like), then OVM will update the exact executable that you call `upgrade` from. 

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
