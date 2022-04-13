Dictionaries can contain key-value pairs of the same type pair.

## `{kt=vt}`
The type of dictionaries containing items of type `vt`, addressable with keys of type `kt`.

## `{=t}`
`{t=t}`.

## `{x=y, z=w, etc}`
A dictionary containing `y` addressable with `x`, `w` addressable with `z`, etc.

## `d#x`
The item in `d` with key `x`.

## `d#x = y`
Set `d#x` to `y`.

## `delete d#x`
Delete `d#x` and return it.

## `d at x`
An array of all keys of `x` in `d`.

## `d has x`
Whether `x` is a key of `d`.

## `d hasnt x`
Whether `x` is not a key of `d`.

## `d.x`
`t#'x'`.

## `d where routine`
A dictionary where `routine` returns `true` for all items in `d`. `routine` takes an item and a key respectively.

## `d via routine`
A copy of `d` where `routine` is applied to all items. `routine` takes an item and a key respectively.

## `some d where routine`
Whether `routine` returns `true` for at least one item in `d`.

## `all d where routine`
Whether `routine` returns `true` for all items in `d`.

## `no d where routine`
Whether `routine` returns `false` for all items in `d`.

## `*d`
Define all keys in `d` as identifiers in the current namespace.

## `x, y, etc = d`
Dictionary destructuring: `x = d#x`, `y = d#y`, etc.