Arrays can only contain objects of the same type. Some of the operation here can obviously only work on dynamic arrays.

## `[t]`
The type of dynamic arrays containing items of type `t`.

## `n [t]`
The type of static arrays with a max of `n` items of type `t`.

## `[x, y, etc]`
A dynamic array containing `x` at index `1`, `y` at index `2`, etc.

## `t [x, y, etc]`
A dynamic array containing items of type `t`: `x` at index `1`, `y` at index `2`, etc.

## `n [x, y, etc]`
A static array of a max of `n` items, containing `x` at index `1`, `y` at index `2`, etc, with the rest, if any, being zero`d out.

## `t n [x, y, etc]`
A static array of a max of `n` items, containing items of type `t`: `x` at index `1`, `y` at index `2`, etc, with the rest, if any, being zero`d out.

## `static [x, y, etc]`
A static array containing `x` at index `1`, `y` at index `2`, etc; and that many items is its max.

## `static t [x, y, etc]`
A static array of type `t`, containing `x` at index `1`, `y` at index `2`, etc; and that many items is its max.

## `'...'B` or `"..."B`
`'...'` as a `u8` array.

## `'...'b` or `"..."b`
`'...'` as an `i8` array.

## `#array`
The length of `array`.

## `array#i`
The item in `array` at `i`, or `#array + i` if `i` is negative.

## `array#a_range`
A slice of `array`.

## `array at x`
An array containing all indices of `x` in `array`.

## `array at subarray`
An array containing all indices of the subarray, `subarray` in `array`.

## `array at x = y`
Set all occurences of `x` in `array` to `y`.

## `array at subarray = new_subarray`
Set all occurences of `subarray` in `array` to `new_subarray`.

## `array..x`
A copy of `array` with `x` at the end.

## `array1..array2`
An array resulting from the concatenation of `array1` and `array2` respectively.

## `array <- x`
Add `x` to the end of `array`.

## `array1 <- array2`
Insert each item in `array2` to the end of `array1`.

## `array#i <<- x`
Add `x` after `array#i`.

## `array1#i <<- array2`
Insert each item in `array2` after `array1#i`.

## `array1#a_range <<- array2`
Insert each item in `array2` in the boundary of `array1#a_range`.

## `array#i = x`
Set `array#i` to `x`.

## `array#a_range = subarray`
Replace `array#a_range` with `subarray`, and return it.

## `less array`
Delete the last item in `array` and return it.

## `delete array#i`
Delete `array#i` and return it.

## `delete array#a_range`
Delete `array#a_range` and return it.

## `array where routine`
An array where `routine` returns `true` for all items in `array`. `routine` takes an item and an index respectively.

## `array via routine`
A copy of `array` where `routine` is applied to all items. `routine` takes an item and an index respectively.

## `array via dictionary`
```
dictionary per k of v
	array#k = v
```

## `some array where routine`
Whether `routine` returns `true` for at least one item in `array`.

## `all array where routine`
Whether `routine` returns `true` for all items in `array`.

## `no array where routine`
Whether `routine` returns `false` for all items in `array`.

## `array down routine`
Start-to-end array reduction.

## `array up routine`
End-to-start array reduction.

## `reverse array`
A reversed copy of `array`.

## `sort array by routine`
A copy of `array` sorted by `routine`.

## `flat(array, depth)`
An array, `new_array`, where all items of all subarrays are inserted into `new_array` in place of the subarrays recursively up to depth `depth`.

## `flat array`
`flat(array, 1)`.

## `x, y, etc = array`
Array destructuring: `x = array#1`, `y = array#2`, etc.