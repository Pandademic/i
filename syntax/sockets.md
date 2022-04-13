The supported network protocols out of the box are `ipv4`, `ipv6`...

## `sock`
The socket type.

## `sock path procedure`
A socket following the protocol in `path`, immediately connected to `path` (see [Paths](#paths)), that calls `procedure` whenever it receives data; `procedure` must be of type:
* `ipv4packet -|` if the protocol is `ipv4`
* `ipv6packet -|` if the protocol is `ipv6`
* `icmppacket -|` if the protocol is `icmp`

## `s#i`
The `i`th character from `s`.

## `s#a_range`
A string slice of `s`.

## `s <- x`
Send `x` to `s`.

## `close s`
Close `s`. Note that sockets are automatically closed when garbage-collected.