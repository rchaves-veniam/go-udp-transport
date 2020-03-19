go-udp-transport
==================

> A libp2p transport implementation for udp, including reuseport socket options.

`go-udp-transport` is an implementation of the [libp2p transport
interface][concept-transport] that streams data over TCP/IP sockets. It is
included by default in the main [`go-libp2p`][go-libp2p] "entry point" module.

## Table of Contents

- [go-udp-transport](#go-udp-transport)
    - [Table of Contents](#table-of-contents)
    - [Install](#install)
    - [License](#license)

## Install

`go-udp-transport` is included as a dependency of `go-libp2p`, which is the most
common libp2p entry point. If you depend on `go-libp2p`, there is generally no
need to explicitly depend on this module.

`go-udp-transport` is a standard Go module which can be installed with:

``` sh
go get github.com/libp2p/go-udp-transport
```


This repo is [gomod](https://github.com/golang/go/wiki/Modules)-compatible, and users of
go 1.11 and later with modules enabled will automatically pull the latest tagged release
by referencing this package. Upgrades to future releases can be managed using `go get`,
or by editing your `go.mod` file as [described by the gomod documentation](https://github.com/golang/go/wiki/Modules#how-to-upgrade-and-downgrade-dependencies).

## License

MIT © Jeromy Johnson

---


<!-- reference links -->
[go-libp2p]: https://github.com/libp2p/go-libp2p
[concept-transport]: https://docs.libp2p.io/concepts/transport/
[interface-host]: https://github.com/libp2p/go-libp2p-core/blob/master/host/host.go
[godoc-libp2p-new]: https://godoc.org/github.com/libp2p/go-libp2p#New
[transport-upgrader]: https://github.com/libp2p/go-libp2p-transport-upgrader
[explain-reuseport]: https://lwn.net/Articles/542629/
[multiaddr]: https://github.com/multiformats/multiaddr
