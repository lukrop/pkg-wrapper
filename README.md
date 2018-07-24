# pkg-wrapper

This is a small wrapper for several package managers with tab-completion.
It provides a simple interface inspired by FreeBSD's [pkg(8)].

[pkg(8)]: https://www.freebsd.org/cgi/man.cgi?query=pkg&sektion=8&manpath=FreeBSD+11.1-RELEASE+and+Ports

## Supported package managers
* XBPS (voidlinux)
* pacman (ArchLinux)
* dpkg (Debian and derivatives)

## Installation

```shell
curl -o /usr/local/bin/pkg https://raw.githubusercontent.com/lukrop/pkg-wrapper/master/pkg
chmod +x /usr/local/bin/pkg
```

## Example usage

Install package *somepackage*
```shell
pkg install somepackage
```

Remove *somepackage*
```shell
pkg remove anotherpkg
```
Upgrade all packages
```shell
pkg upgrade
```

Find package to which /some/file belongs
```shell
pkg which /some/file
```

Hold *somepackage* at current version
```shell
pkg hold somepackage
```
See `pkg help` for more.

