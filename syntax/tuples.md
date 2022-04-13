Tuples can contain objects of different types, but are immudictionary. Tuple items can be addressable by non-integer keys.

## `(t, u=v, etc)`
The type of tuples containing an integer-indexed item of type `t`, an item of type `v`, addressable by keys of type `u`, etc.

## `x, y=z, etc`
A tuple containing `x` at index `1`, `z`, addressable with `y`, etc.

## `,x` or `x,`
A tuple containing `x` at index `1`.

## `#t`
The length of `t`.

## `t#i`
The item in `t` at `i`, or `#t + i` if `i` is negative.

## `t#x`
The item in `t` with key `x`.

## `t.x`
`t#'x'`.

## `*t`
Define all keys in `t` as variables in the current namespace.

## `x, y, etc = t`
Tuple destructuring: `x = t#1`, `y = t#2`, etc.