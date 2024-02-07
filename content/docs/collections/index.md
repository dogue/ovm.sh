+++
title = "Collections"
template = "docs/page.html"
date = "2024-02-06"
weight = 20
[extra]
toc = true
+++

After install or when switching the active Odin version, OVM will create a few symbolic links inside the `~/.ovm` directory to make working with Odin's package collections a bit more convenient.

* `<version>/core` => `.ovm/collections/core`
* `<version>/vendor` => `.ovm/collections/vendor`
* `.ovm/collections/shared` => `<version>/shared`

---

The reason for this is that the Odin LSP (OLS) needs the path to the collections to be defined in `ols.json`. With these symlinks, you can simply point your config to `$HOME/.ovm/collections/<collection>` and reuse the same config for every project, regardless of which version is active.

The `shared` directory is intended as a place for you to sort of "self-vendor" libraries. Putting an Odin library here will make it available to all of your projects. This directory is empty by default and would normally get removed each time you update (or replaced each time you change versions), and thus we use a directory that is persistent, and symlink it in as needed.
