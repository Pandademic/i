Bit fields can be operands of bitwise operators.

## `bitf`
The bit field type.

## `0b[x, y=z, etc]`
A bit field containing `x`, `z`, etc—which are binary literals without `0b`—as bits, with `z` being addressable as a slice of the bit field, with the non-integer key, `y`. Those kinds of slices are called divisions.

## `bf#i`
Whether the `i`th bit in `bf` is set.

## `bf#a_range`
A slice of `bf`.

## `bf#x`
The division in `bf`, with the non-integer key, `x`.

## `bf1..bf2`
The bitfield resulting from the concatenation of `bf1` and `bf2` respectively.

## `bf#i = falsy_object`
Clear `bf#i`.

## `bf#i = truthy_object`
Set `bf#i`.

## `bf#i <<- x`
Insert all the bits in `x` after `bf#i`.

## `bf#a_range <<- x`
Insert all the bits in `x` in the boundary of `bf#a_range`.