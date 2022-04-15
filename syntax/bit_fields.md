Bit fields can be operands of bitwise operators.

## `bitf`
The bit field type.

## `0b[x, k=y, etc]`
A bit field containing `x`, `y`, etc—which must be binary literals without `0b`—as bits, with `y` being addressable as a slice of the bit field, with the non-integer key, `k`. Those kinds of slices are called divisions.

## `bf#i`
Whether the `i`th bit in `bf` is set.

## `bf#r`
A slice of `bf` in range `r`.

See *ranges.md*.

## `bf#k`
The division in `bf`, with the non-integer key, `k`.

## `bf1..bf2`
The bitfield resulting from the concatenation of `bf1` and `bf2` respectively.

## `bf#i <- x`
Insert all the bits in `x` after `bf#i`.

## `bf1#i <- bf2`
Insert all the bits in bit field `bf2` after `bf#i`.

## `bf#i = x`
If `x` is truthy, set the `i`th bit in `bf`. Clear it otherwise.