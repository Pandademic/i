## `icmppacket`
The ICMP packet type.

## `icmppacket c`
An ICMP packet from the collection, `c`.

## `p.type`
`p`'s type.

## `p.code`
`p`'s code.

## `p.checksum`
`p`'s checksum.

## `p.body`
`p`'s rest of header.

## `p.ipheader`
`p`'s IP header; available for some packet types and codes.

## `p.plbyte`
`p`'s first byte of the IP packet's payload; available for some packet types and codes.

## `p.rediraddr`
`p`'s redirect IP address; available for some packet types and codes.

## `p.id`
`p`'s identifier; available for some packet types and codes.

## `p.seqnumber`
`p`'s sequence number; available for some packet types and codes.

## `p.otime`
`p`'s originate timestamp time; available for some packet types and codes.

## `p.rtime`
`p`'s receive timestamp time; available for some packet types and codes.

## `p.ttime`
`p`'s transmit timestamp time; available for some packet types and codes.

## `p.mask`
`p`'s address mask; available for some packet types and codes.

## `p.nexthopmtu`
`p`'s next-hop MTU; available for some packet types and codes.