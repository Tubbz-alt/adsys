# adsys
Active Directory bridging toolset

## Usage

### User commands

#### adsysctl

AD integration client

##### Synopsis

Active Directory integration bridging toolset command line tool.

```
adsysctl COMMAND [flags]
```

##### Options

```
  -c, --config string   use a specific configuration file
  -h, --help            help for adsysctl
  -s, --socket string   socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int     time in seconds before cancelling the client request when the server gives no result. 0 for no timeout. (default 30)
  -v, --verbose count   issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysctl completion

Generates bash completion scripts

##### Synopsis

To load completion run

. <(adsysctl completion)

To configure your bash shell to load completions for each session add to your ~/.bashrc or ~/.profile:

. <(adsysctl completion)


```
adsysctl completion [flags]
```

##### Options

```
  -h, --help   help for completion
```

##### Options inherited from parent commands

```
  -c, --config string   use a specific configuration file
  -s, --socket string   socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int     time in seconds before cancelling the client request when the server gives no result. 0 for no timeout. (default 30)
  -v, --verbose count   issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysctl policy

Policy management

##### Synopsis

Policy management

```
adsysctl policy COMMAND [flags]
```

##### Options

```
  -h, --help   help for policy
```

##### Options inherited from parent commands

```
  -c, --config string   use a specific configuration file
  -s, --socket string   socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int     time in seconds before cancelling the client request when the server gives no result. 0 for no timeout. (default 30)
  -v, --verbose count   issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysctl policy update

Updates/Create a policy for current user or given user with its kerberos ticket

##### Synopsis

Updates/Create a policy for current user or given user with its kerberos ticket

```
adsysctl policy update [USER KERBEROS_TICKET_PATH] [flags]
```

##### Options

```
  -h, --help      help for update
  -m, --machine   machine updates the policy of the computer.
```

##### Options inherited from parent commands

```
  -c, --config string   use a specific configuration file
  -s, --socket string   socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int     time in seconds before cancelling the client request when the server gives no result. 0 for no timeout. (default 30)
  -v, --verbose count   issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysctl service

Service management

##### Synopsis

Service management

```
adsysctl service COMMAND [flags]
```

##### Options

```
  -h, --help   help for service
```

##### Options inherited from parent commands

```
  -c, --config string   use a specific configuration file
  -s, --socket string   socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int     time in seconds before cancelling the client request when the server gives no result. 0 for no timeout. (default 30)
  -v, --verbose count   issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysctl service cat

Print service logs

##### Synopsis

Print service logs

```
adsysctl service cat [flags]
```

##### Options

```
  -h, --help   help for cat
```

##### Options inherited from parent commands

```
  -c, --config string   use a specific configuration file
  -s, --socket string   socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int     time in seconds before cancelling the client request when the server gives no result. 0 for no timeout. (default 30)
  -v, --verbose count   issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysctl service stop

Requests to stop the service once all connections are done

##### Synopsis

Requests to stop the service once all connections are done

```
adsysctl service stop [flags]
```

##### Options

```
  -f, --force   force will shut it down immediately and drop existing connections.
  -h, --help    help for stop
```

##### Options inherited from parent commands

```
  -c, --config string   use a specific configuration file
  -s, --socket string   socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int     time in seconds before cancelling the client request when the server gives no result. 0 for no timeout. (default 30)
  -v, --verbose count   issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysctl version

Returns version of client and service

##### Synopsis

Returns version of client and service

```
adsysctl version [flags]
```

##### Options

```
  -h, --help   help for version
```

##### Options inherited from parent commands

```
  -c, --config string   use a specific configuration file
  -s, --socket string   socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int     time in seconds before cancelling the client request when the server gives no result. 0 for no timeout. (default 30)
  -v, --verbose count   issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysd

AD integration daemon

##### Synopsis

Active Directory integration bridging toolset daemon.

```
adsysd COMMAND [flags]
```

##### Options

```
  -D, --ad-domain string   AD domain to use. Empty to let ADSys parsing sssd.conf.
  -S, --ad-server string   URL of the Active Directory server. Empty to let ADSys parsing sssd.conf.
  -c, --config string      use a specific configuration file
  -h, --help               help for adsysd
  -s, --socket string      socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int        time in seconds without activity before the service exists. 0 for no timeout. (default 120)
  -v, --verbose count      issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysd completion

Generates bash completion scripts

##### Synopsis

To load completion run

. <(adsysd completion)

To configure your bash shell to load completions for each session add to your ~/.bashrc or ~/.profile:

. <(adsysd completion)


```
adsysd completion [flags]
```

##### Options

```
  -h, --help   help for completion
```

##### Options inherited from parent commands

```
  -D, --ad-domain string   AD domain to use. Empty to let ADSys parsing sssd.conf.
  -S, --ad-server string   URL of the Active Directory server. Empty to let ADSys parsing sssd.conf.
  -c, --config string      use a specific configuration file
  -s, --socket string      socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int        time in seconds without activity before the service exists. 0 for no timeout. (default 120)
  -v, --verbose count      issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

#### adsysd version

Returns version of service and exits

##### Synopsis

Returns version of service and exits

```
adsysd version [flags]
```

##### Options

```
  -h, --help   help for version
```

##### Options inherited from parent commands

```
  -D, --ad-domain string   AD domain to use. Empty to let ADSys parsing sssd.conf.
  -S, --ad-server string   URL of the Active Directory server. Empty to let ADSys parsing sssd.conf.
  -c, --config string      use a specific configuration file
  -s, --socket string      socket path to use between daemon and client. Can be overriden by systemd socket activation. (default "/tmp/socket.default")
  -t, --timeout int        time in seconds without activity before the service exists. 0 for no timeout. (default 120)
  -v, --verbose count      issue INFO (-v), DEBUG (-vv) or DEBUG with caller (-vvv) output
```

### System commands

Those commands are hidden from help and should primarily be used by the system itself.

