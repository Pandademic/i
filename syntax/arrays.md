Arrays can only contain objects of the same type. Some of the operation here can obviously only work on dynamic arrays.

## `[T]`
The type of dynamic arrays containing items of type `T`.

## `n [T]`
The type of static arrays with a max of `n` items of type `T`.

## `[x, y, ...]`
A dynamic array containing `x` at index `1`, `y` at index `2`, etc.

## `T [x, y, ...]`
A dynamic array containing items of type `T`: `x` at index `1`, `y` at index `2`, etc.

## `n [x, y, ...]`
A static array of a max of `n` items, containing `x` at index `1`, `y` at index `2`, etc, with the rest, if any, being zero`d out.

## `T n [x, y, ...]`
A static array of a max of `n` items, containing items of type `T`: `x` at index `1`, `y` at index `2`, etc, with the rest, if any, being zero`d out.

## `static [x, y, ...]`
A static array containing `x` at index `1`, `y` at index `2`, etc; and that many items is its max.

## `static T [x, y, ...]`
A static array of type `T`, containing `x` at index `1`, `y` at index `2`, etc; and that many items is its max.

## `#a`
The length of `a`.

## `a#i`
The item in `array` at index `i` or `#a + i` if `i` is negative.

## `a#r`
A slice of `a` in range `r`.

See *ranges.md*.

## `a at x`
An array of all indices of `x` in `a`.

## `a at sa`
An array of all indices of subarray `sa` in `a`.

## `a at x = y`
Set all occurences of `x` in `a` to `y`.

## `a at sa = y`
Set all occurences of subarray `sa` in `a` to new subarray `y`.

## `a..x`
A copy of `a` with `x` at the end.

## `x..a`
A copy of `a` with `x` at the beginning.

## `a1..a2`
An array resulting from the concatenation of `a1` and `a2` respectively.

## `a <- x`
Insert `x` at the end of `a`.

## `x -> a`
Insert `x` at the beginning of `a`.

## `a1 <- a2`
Insert each item in `a2` to the end of `a1`.

## `a2 -> a1`
Insert each item in `a2` to the beginning of `a1`.

## `a#i <- x`
Insert `x` after `a#i`.

## `x -> a#i`
Insert `x` before `a#i`.

## `a1#i <- a2`
Insert each item in `a2` after `a1#i`.

## `a2 -> a1#i`
Insert each item in `a2` before `a1#i`.

## `a#i = x`
Set `a#i` to `x`.

## `a#r = x`
Replace `a#r` with `x`, and return it.

See *ranges.md*.

## `delete a#i`
Delete the `i`-th item in `a` and return it.

## `delete a#r`
Delete all of `a`'s items in range `r` and return them as an array of the same type.

## `less a`
Delete the last item in `a` and return it.

## `n less a`
Delete the last `n` items in `a` and return them as an array of the same type.

## `a where f`
An array where `f` returns `true` for all items in `a`. `f` must take an item and index respectively.

See *routines.md*.

## `f a`
An array where `f` is applied to all items in `a`. `f` must take an item and index respectively.

See *routines.md*.

## `a via d`
An array where each item in `a` is replaced with the value with the same index/key in dictionary `d`.

See *dictionaries.md*.

## `some a`
Whether at least one item in `a` is truthy.

## `notsome a`
Whether at least one item in `a` is falsy.

## `some n a`
Whether exactly `n` items in `a` are truthy.

## `notsome n a`
Whether exactly `n` items in `a` are falsy.

## `some r a`
Whether the number of truthy items in `a` is in range `r`.

## `notsome r a`
Whether the number of falsy items in `a` is in range `r`.

## `all a`
Whether all items in `a` are truthy.

## `no a`
Whether all items in `a` are falsy.

## `a down f`
An array where `a` is reduced by function `f` from beginning to end.

## `a up f`
An array where `a` is reduced by function `f` from end to beginning.

## `reversed a`
An array where the order of `a`'s items is reversed.

## `a by f`
An array where `a`'s items are sorted by function `f` which must be of one of these types: `(T, T) => bool`, `(int, int) => bool` or `((int, T), (int, T)) => bool` where `T` is the item type, and `int` is the index's. Returning `true` means sorting the item of the first argument after the second's.

See *functions.md* and *tuples.md*.

## `flat(a, n)`
An array where all items of all subarrays in `a` are inserted into it in their place recursively up to depth `n`.

## `flat a`
An array where all items of all subarrays in `a` are inserted into it in their place.

Equivalent to `flat(a, 1)`.

## `x, y, etc = a`
Array destructuring: `x = a#1`, `y = a#2`, etc.