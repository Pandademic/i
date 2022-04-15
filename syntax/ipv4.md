# IPv4 Packets

IPv4 packets and IP options are mutable.

## `ipv4packet`
The IPv4 packet type.

## `ipv4packet c`
An IPv4 packet from the collection, `c`.

## `#p`
The size of `p` in bytes.

## `p.headerlen`
The size of `p`'s header in bytes.

## `p.dscp`
`p`'s DSCP.

## `p.ecn`
`p`'s ECN.

## `p.id`
`p`'s Identification.

## `p.df`
Whether `p`'s DF flag is set.

## `p.mf`
Whether `p`'s MF flag is set.

## `p.offset`
`p`'s fragment offset.

## `p.ttl`
`p`'s TTL.

## `p.protocol`
`p`'s protocol; can be `ICMP`, `IGMP`, `TCP`, `UDP`, `ENCAP`, `OSPTF` or `SCTP`, which are of type `ipprotocol`.

See *enumerators_and_enumerals.md*.

## `p.checksum`
`p`'s header checksum.

## `p.srcaddr`
`p`'s source address.

## `p.destaddr`
`p`'s destination address.

## `p.options`
`p`'s options.

## `#p.options`
`p`'s number of options.

## `p.payload`
`p`'s payload.

# IPv4 Options

## `ipopt`
The IPv4 option type.

## `ipopt c`
An IPv4 option from the collection, `c`.

## `#o`
The option, `o`'s length.

## `o.copied`
Whether `o`'s Copied field is set.

## `o.class`
`o`'s class.

## `o.number`
`o`'s number.

## `o.type`
`o`'s type; can only be `EOOL`, `NOP`, `SEC`, `RR`, `ZSU`, `MTUP`, `MTUR`, `ENCODE`, `QS`, `EXP`, `TS`, `TR`, `EXP`, `SEC`, `LSR`, `E-SEC`, `CIPSO`, `SID`, `SSR`, `VISA`, `IMITD`, `EIP`, `ADDEXT`, `RTRALT`, `SDB`, `DPS`, `UMP`, `EXP`, `FINN` or `EXP`, which are of type `ipopttype`.

See *enumerators_and_enumerals.md*.

## `o.data`
`o`'s data.

# IPv4 Addresses

## `ipv4addr`
The IPv4 address type.

## `ipv4addr c`
An IPv4 address from the collection, `c`.

## `a#i`
The `i`th of the 4 divided numbers of the address, `a`.

## `a#a_range`
An array of the divided numbers of `a` in range `r`.

## `a#i = x`
Set `a#i` to `x`.

## `a#r = x`
Set `a#r` to the array, `x`.