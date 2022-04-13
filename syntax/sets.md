Sets can only contain non-duplicate objects of the same type, and are mudictionary. Some of the operation here can obviously only work on dynamic sets.

## `{t}`
The type of dynamic sets containing items of type `t`.

## `n {t}`
The type of static sets of a max of `n` items of type `t`.

## `{,}` or `n {,}`
An empty set with a context-dependent type.

## `t {,}` or `t n {,}`
An empty set that can contain items of type `t`.

## `{x, y, etc}`
A dynamic set containing `x`, `y`, etc, in no particular order.

## `t {x, y, etc}`
A dynamic set containing items of type `t`: `x`, `y`, etc, in no particular order.

## `n {x, y, etc}`
A dynamic set of a max of `n` items, containing `x`, `y`, etc, in no particular order, with the rest, if any, being zero'd out.

## `t n {x, y, etc}`
A dynamic set of a max of `n` items, containing items of type `t`: `x`, `y`, etc, in no particular order, with the rest, if any, being zero'd out.

## `static {x, y, etc}`
A static set containing `x`, `y`, etc, in no particular order; that many items is its max.

## `static t {x, y, etc}`
A static set containing items of type `t`: `x`, `y`, etc, in no particular order; that many items is its max.

## `#s`
The length/cardinality of `s`.

## `s <- x`
Add `x` to `s`.

## `s has x`
Whether `x` is in `s`.

## `s hasnt x`
Whether `x` is not in `s`.

## `delete set at x`
Delete the item, `x`, from `set`.

## `s1 <= s2`
Whether `s1` is a subset of `s2'

## `s1 < s2`
Whether `s1` is a proper subset of `s'

## `s1 >= s2`
Whether `s1` is a superset of `s2'

## `s1 > s2`
Whether `s1` is a proper superset of `s2'

## `s1 + s2`
The union of `s1` and `s2`.

## `s1 & s2`
The intersection of `s1` and `s2`.

## `s1 ^ s2`
The symmetric difference of `s1` and `s2`.

## `s1 - s2`
The relative complement of `s1` and `s2`.