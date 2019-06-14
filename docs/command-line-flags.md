# Command Line Flags

Command line flags override the confd [configuration file](configuration-guide.md).

```
confd -h
```

use etcdv3 as default etcd, do not support etcd v2.

```Text
Usage of confd:
  -backend string
      backend to use (default "etcd")
  -basic-auth
      Use Basic Auth to authenticate (only used with -backend=etcd)
  -client-ca-keys string
      client ca keys
  -client-cert string
      the client cert
  -client-key string
      the client key
  -confdir string
      confd conf directory (default "/etc/confd")
  -config-file string
      the confd config file (default "/etc/confd/confd.toml")
  -file value
      the YAML file to watch for changes (only used with -backend=file)
  -filter string
      files filter (only used with -backend=file) (default "*")
  -interval int
      backend polling interval (default 600)
  -keep-stage-file
      keep staged files
  -log-level string
      level which confd should log messages
  -node value
      list of backend nodes
  -noop
      only show pending changes
  -onetime
      run once and exit
  -password string
      the password to authenticate with (only used etcd backends)
  -prefix string
      key path prefix
  -scheme string
      the backend URI scheme for nodes retrieved from DNS SRV records (http or https) (default "http")
  -secret-keyring string
      path to armored PGP secret keyring (for use with crypt functions)
  -separator string
      the separator to replace '/' with when looking up keys in the backend, prefixed '/' will also be removed (only used with -backend=redis)
  -srv-domain string
      the name of the resource record
  -srv-record string
      the SRV record to search for backends nodes. Example: _etcd-client._tcp.example.com
  -sync-only
      sync without check_cmd and reload_cmd
  -username string
      the username to authenticate as (only used with etcd backends)
  -version
      print version and exit
  -watch
      enable watch support
```

> The -scheme flag is only used to set the URL scheme for nodes retrieved from DNS SRV records.
