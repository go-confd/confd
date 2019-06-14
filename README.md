# confd

Forked from [kelseyhightower/confd](https://travis-ci.org/kelseyhightower/confd)

`confd` is a lightweight configuration management tool focused on:

* keeping local configuration files up-to-date using data stored in [etcd](https://github.com/coreos/etcd), [redis](http://redis.io), or env vars and processing [template resources](docs/template-resources.md).
* reloading applications to pick up new config file changes

## Community

* IRC: `#confd` on Freenode
* Mailing list: [Google Groups](https://groups.google.com/forum/#!forum/confd-users)
* Website: [go-confd.github.io](http://go-confd.github.io)

## Building

Go 1.11+ is required to build confd, which uses the new go mod.

```
$ mkdir -p $GOPATH/src/github.com/kelseyhightower
$ git clone https://github.com/go-confd/confd.git
$ cd $PWD/confd
$ make
```

You should now have confd in your `bin/` directory:

```
$ ls bin/
confd
```

## Getting Started

Before we begin be sure to [download and install confd](docs/installation.md).

* [quick start guide](docs/quick-start-guide.md)

## Next steps

Check out the [docs directory](docs) for more docs.
