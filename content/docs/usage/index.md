+++
title = "Usage"
weight = 10
template = "docs/page.html"
[extra]
toc = true
+++

## Install Odin

```sh
ovm install <version>
# or
ovm i <version>
```

Use `install` or `i` to download a specific monthly release of Odin. To install the latest release, use "latest" or leave the version empty. To install the bleeding edge from the master branch, use "master".

### Install OLS with OVM

OVM can also install the Odin Language Server for you. To install OLS, pass the `-l/--lsp` flag to `ovm install`.

```sh
ovm i master -l
# or
ovm i master --lsp
```

---

## Switch the active Odin version

```sh
ovm use <version>
# or
ovm switch <version>
```

Either `use` or `switch` can be used to switch between installed Odin versions.

```sh
ovm use dev-2024-02
```

---

## List installed Odin versions

```sh
ovm ls
# or
ovm list
```

Use `ls` or `list` to see a list of all Odin versions currently installed on your system.

### List versions available for download

```sh
ovm ls --remote
```

The `-r/--remote` flag will list Odin releases that are available to download rather than those installed locally.

---

## Remove an Odin version

```sh
ovm rm dev-2023-08
```

Use `remove` or `rm` to uninstall a local version.

---

## Upgrade your OVM installation

```sh
ovm upgrade
```

OVM will check your current version against the latest and attempt to update itself if there is a newer version available. It should work regardless of where OVM is located, though if it's in a privileged directory you may have to prepend this command with `sudo`.

---

## Toggle output colors

```sh
ovm colors
```

OVM maintains a persistent setting for whether colors in output should be enabled. The `colors` command will display the current setting and prompt you to toggle it, if you wish.

---

## CLI help

```sh
ovm help
```

This will print the built-in help text.

---

## Option flags

* `-v/--verbose` enable additional informational output
