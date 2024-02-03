+++
render = true
title = "Odin Version Manager"
extra.lead = "Easily install/upgrade/switch between different versions of Odin."
extra.url = "/docs/install"
+++

### What Is It?

Odin Version Manager (ovm) is a tool for managing your Odin installs. With the compiler under heavy development, Odin is bound to continue changing. While it's great that Odin is growing so quickly, this can lead to headaches when you may need a specific version for a particular project, or want to stay up to date with the latest.

### Why Should I Use OVM?

While Odin is still pre-1.0, if you're going to stay up-to-date with the master branch, you're going to be downloading Odin quite often. You could do it manually, and in fact cloning the repository *is* the [recommended](https://odin-lang.org/docs/install/#clone-or-download-odin-binaries) approach. However that can get tedious if you plan to update frequently. Another option is to install OVM and run `ovm i master` every time you want to update. `ovm` is a static binary under a [permissive license](https://mit-license.org/). Its only dependency is `tar` on Unix-based systems.
