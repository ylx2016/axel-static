<!-- binaries -->

## axel v2.17.14 static binaries

Built from the official release tarball (sha256 `938ee7c8c478bf6fcc82359bbf9576f298033e8b13908e53e3ea9c45c1443693`).

```console
$ file axel-*
axel-aarch64-linux-musl: ELF 64-bit LSB executable, ARM aarch64, version 1 (SYSV), statically linked, stripped
axel-x86_64-linux-musl:  ELF 64-bit LSB executable, x86-64, version 1 (SYSV), statically linked, no section header

$ ./axel-x86_64-linux-musl --version | sed -n 1p
Axel 2.17.14 (linux-musl)

$ qemu-aarch64-static ./axel-aarch64-linux-musl --version | sed -n 1p
Axel 2.17.14 (linux-musl)

$ sha256sum axel-*
8380cae1383ff079dbcfb704c482cce374730cb8d901d87cffbc688ea24b1a8e  axel-aarch64-linux-musl
63a244f166d2824d578a7086a789bcd865b01d720d9af9d439ea65ccf7804405  axel-x86_64-linux-musl
```
