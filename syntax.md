# Table of Contents

* [Comments](#comments)
* [Null](#null)
* [Numbers](#numbers)
* [Booleans](#booleans)
* [Collections](#collections)
* [Arrays](#arrays)
* [Ranges](#ranges)
* [Tuples](#tuples)
* [Sets](#sets)
* [Dictionaries](#dictionaries)
* [Matrices](#matrices)
* [Strings](#strings)
* [Patterns](#patterns)
* [Formats](#formats)
* [Enumerators & Enumerals](#enumerators--enumerals)
* [Bit Fields](#bit-fields)
* [Versions](#versions)
* [Memory Blocks](#memory-blocks)
* [Paths](#paths)
* [Files](#files)
* [Stdout, Stdin & Stderr](#stdout-Stdin--Stderr)
* [Streams](#streams)
* [Sockets](#sockets)
* [IPv4 Packets](#iPv4-packets)
* [IPv4 Options](#iPv4-options)
* [IPv4 Addresses](#iPv4-addresses)
* [IPv6 Packets](#iPv6-packets)
* [IPv6 Addresses](#iPv6-addresses)
* [ICMP Packets](#iCMP-packets)
* [ICMPv6 Packets](#iCMPv6-packets)
* [Times](#times)
* [Progresses](#progresses)
* [Exceptions](#exceptions)
* [Routines](#routines)
* [Classes](#classes)
* [Identifiers](#identifiers)
* [Control Flow](#control-flow)
* [Blocks](#blocks)
* [Conversions](#conversions)
* [Falsy Objects](#falsy-objects)
* [External Code](#external-code)
* [Modules](#modules)
* [Miscellaneous](#miscellaneous)

# Comments

## `\...`
Line comment.

## `\(...\)`
Block comment. Note that you can easily uncomment a block comment by deleting `(`.

# Null

## `null`
The null type, or its instance.

# Numbers

Number types:
* `u8` — the unsigned 8-bit integer type
* `u16` — the unsigned 16-bit integer type
* `u32` — the unsigned 32-bit integer type
* `u64` — the unsigned 64-bit integer type
* `i8` — the signed 8-bit integer type
* `i16` — the signed 16-bit integer type
* `i32` — the signed 32-bit integer type
* `i64` — the signed 64-bit integer type
* `nat` — the unsigned arch-sized integer type
* `int` — the signed arch-sized integer type
* `real` — the single- or double-precision float type, depending on the arch
* `complex` — the single- or double-precision complex number type, depending on the arch
* `bignat` — the unsigned arbitrary-precision integer type
* `bigint` — the signed arbitrary-precision integer type
* `bigreal` — the arbitrary-precision float type
* `bigcomplex` — the arbitrary-precision complex number type

Numeral examples:
* `-0b101` — a binary literal
* `0 + 0o377i` — a complex numeral from a decimal and an octal; `0+` can be omitted here.
* `1_000_000` — like 1,000,000
* `2.9979***8` — a decimal multiplied by 10 to the 8th (see [x *** y](#x--y-2))
* `0x4.0f` — a hexadecimal with a point; note here that all kinds of numerals can have points, not just decimals

Integer numerals are `int`s/`bigint`s, and floating-point numerals are `real`s/`bigreal`s.

Names referring to integers can be used in floating-point literals—e.g. `2.x`; in this example, if `x` is negative, the whole number will be negative, because `2` is positive, and vice versa.

## `t`
The number type, `t`, or an instance of it, set to `0`.

## `min t`
The smallest number of type `t`; can't be used with arbitrary-precision types.

## `max t`
The biggest number of type `t`; can't be used with arbitrary-precision types.

## `-x`
Negation.

## `x - y`
Subtraction.

## `x + y`
Addition.

## `x * y` or `x y`
Multiplication.

## `x ** y`
Exponentiation.

## `x *** y`
* `x * 2**y` for binary literals
* `x * 8**y` for octals
* `x * 10**y` for decimals
* `x * 16**y` for hexadecimals

## `x / y`
Division.

## `x // y`
The `x`th root of `y`.

## `//x`
`2//x`.

## `x % y`
Modulo.

## `x & y`
Bitwise AND.

## `x | y`
Bitwise OR.

## `x ^ y`
Bitwise XOR.

## `x << y`
Left arithmetic shift.

## `x >> y`
Right arithmetic shift.

## `x <<< y`
Left logical shift.

## `x >>> y`
Right logical shift.

## `x <-< y`
Left bitwise rotation.

## `x >-> y`
Right bitwise rotation.

## `x#i`
Whether the `i`th bit in `x` is set.

## `x#a_range`
A bit field from `x` in the boundary of `a_range`.

## `x#i = falsy_object`
Clear `x#i`.

## `x#i = truthy_object`
Set `x#i`.

## `x#i <<- o`
Insert all the bits in `o` after `x#i`.

## `x#a_range <<- o`
Insert all the bits in `o` in the boundary of `x#a_range`.

## `|x|`
The absolute value of `x`.

## `log x`
The natural logarithm of `x`.

## `log#y x`
The base-`y` logarithm of `x`.

## `sin x`
The sine of `x`.

## `sinh x`
The hyperbolic sine of `x`.

## `asin x`
The arcsine of `x`.

## `asinh x`
The hyperbolic arcsine of `x`.

## `cos x`
The cosine of `x`.

## `cosh x`
The hyperbolic cosine of `x`.

## `acos x`
The arccosine of `x`.

## `acosh x`
The hyperbolic arccosine of `x`.

## `tan x`
The tangent of `x`.

## `tanh x`
The hyperbolic tangent of `x`.

## `atan x`
The arctangent of `x`.

## `atanh x`
The hyperbolic arctangent of `x`.

## `floor x`
The largest integer `i`, where `i <= x`.

## `ceil x`
The smallest integer `i`, where `i >= x`.

## `round x`
`x` rounded to the nearest integer.

## `trunc x`
`x` without the fractional part.

## `binstr x`
`x` as a binary literal in a string.

## `octstr x`
`x` as an octal in a string.

## `decstr x` or `str x`
`x` as a decimal in a string.

## `hexstr x`
`x` as a hexadecimal in a string.

## `sum numbers`
The sum of all numbers in `numbers`, or `0` if `numbers` is empty.

## `hypot numbers`
The hypotenuse of all numbers in `numbers`, or `0` if `numbers` is empty..

## `max numbers`
The largest number in `numbers`, or `0` if `numbers` is empty.

## `min numbers`
The smallest number in `numbers`, or `0` if `numbers` is empty.

# Booleans

## `bool`
The boolean type.

## `false`
False.

## `true`
True.

## `x == y`
Whether `x` is equal to `y`.

## `x === y`
Whether `x` is equal to `y` and they're the same type.

## `x != y`
Whether `x` is not equal to `y`.

## `x !== y`
Whether `x` is not equal to `y` and they're the same type.

## `x is y`
Whether `x` and `y` refer to the same object.

## `x isnt y`
Whether `x` and `y` don't refer to the same object.

## `x < y`
Whether `x` is strictly less than `y`.

## `x <= y`
Whether `x` is less than or equals `y`.

## `x > y`
Whether `x` is strictly greater than `y`.

## `x >= y`
Whether `x` is greater than or equals `y`.

## `x < y < z`
`x < y and y < z`.

## `x <= y < z`
`x <= y and y < z`.

## `x < y <= z`
`x < y and y <= z`.

## `x <= y <= z`
`x <= y and y <= z`.

## `x > y > z`
`x > y and y > z`.

## `x >= y > z`
`x >= y and y > z`.

## `x > y >= z`
`x > y and y >= z`.

## `x >= y >= z`
`x >= y and y >= z`.

## `not x`
`false` if `x` is true; `true` otherwise.

## `x and y`
Whether both `x` and `y` are true.

## `x or y`
Whether `x` or `y` is true.

## `x xor y`
Whether only one of `x` and `y` is true.

## `invert x`
`x = not x`.

# Collections

The types of collections are [arrays](#arrays), [ranges](#ranges), [tuples](#tuples), [sets](#sets), [dictionaries](#dictionaries), [matrices](#matrices), [strings](#strings), [enumerators](#enumerators--enumerals), [bit fields](#<#Bit Fields>), [paths](#paths), [files](#files), [streams](#streams) and [classes](#classes). All of them are iterable (see [Streams](#streams)).

Doing a scalar operation on an array, tuple, dictionary, matrix or string, with scalar items result in a new one where the operation is done on all of its items.

## `join collection with separator`
A string containing the stringified versions of all items from `collection` in order, separated with `separator`, which can be a pattern (see [Patterns](#patterns)).

## `join collection`
`join collection with x`, where `x` is a collection-type-based separator: `', '` for most collection types.

## `str collection`
`join collection with ''`.

## `* collection`
Expand `collection` depending on the expression being expanded in.

# Arrays

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

# Ranges

Ranges can only contain integers. They're immudictionary.

## `range`
The range type.

## `x..y..z`
Range from `x` to `z` each `y` steps.

## `x..y...z`
`x..y..(x + z)`. 

## `x...y..z`
`x..(x + y)..z`. 

## `x...y...z`
`x..(x + y)...(x + z)`. 

## `x..y..`
`x..y..inf`.

## `..y..z`
`0..y..z`.

## `x..z`
`x..1..z`.

## `x..` or `x+`
`x..inf`.

## `..z` or `z-`
`0..z`.

## `r#i`
The integer #`i` in `r`.

## `x, y, etc = r`
Range destructuring: `x = r#1`, `y = r#2`, etc.

# Tuples

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

# Sets

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

# Dictionaries

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

# Matrices

Matrices are static. The mathematical operations here can only work on number matrices. Matrices whose rows only contain one item each are called vectors.

## `n [;t]` or `n [t;]`
The type of matrices of a max of `n` items of type `t`.

## `n [;]`
An empty matrix with a context-dependent type.

## `t n [;]`
An empty matrix that can contain items of type `t`.

## `[a11, a12, etc; a21, a22, etc; etc]`
A matrix; the number of items in `a11, a12, etc; a21, a22, etc; etc` is its max.

## `n [a11, a12, etc; a21, a22, etc; etc]`
A matrix of a max of `n` items.

## `t n [a11, a12, etc; a21, a22, etc; etc]`
A dynamic matrix of a max of `n` items of type `t`.

## `[;x]` or `[x;]`
A matrix with one item, `x`.

## `[x; y; z]`
A vector.

## `#m`
The number of items in `m`.

## `m#i`
If `i` is a terminal index: an item in `m`; otherwise a submatrix of `m`.

## `m#(i, j, etc)`
If `(i, j, etc)` is a terminal index: an item in `m`; otherwise a submatrix of `m`.

## `m#(i, j, etc) = x`
Set `m#(i, j, etc)` to `x`.

## `transpose m`
A transposed copy of `m`.

## `m1 * m2` or `m1 m2`
Matrix multiplication.

## `[a11, a12, etc; a21, a22, etc; etc] = m`
Vector destructuring: `a11, a12 = m#1`, `a21, a22 = m#2`, etc.

## `v.x`, `v.s` or `v.r`
`v#1` where `v` is a vector.

## `v.y`, `v.t` or `v.g`
`v#2`.

## `v.z`, `v.u` or `v.b`
`v#3`.

## `v.w`, `v.v` or `v.a`
`v#4`.

## `|v|`
The magnitude of `v`.

## `norm v`
A normalized copy of `v`.

## `v1 dot v2`
The dot product of `v1` and `v2`.

## `v1 cross v2`
The cross product of `v1` and `v2`.

## `v1 theta v2`
The angle between `v1` and `v2`.

## `[x; y; etc] = v`
Vector destructuring: `x = v#x`, `y = v#y`, etc.

# Strings

Some of the operation here can obviously only work on dynamic strings.

## `str8`
The type of dynamic strings containing 8-bit characters.

## `str16`
The type of dynamic strings containing 16-bit characters.

## `str32`
The type of dynamic strings containing 32-bit characters.

## `str64`
The type of dynamic strings containing 64-bit characters.

## `str`
Expands to an appropriate string type depending on the expression; e.g. `str[u8 0]` becomes `str8'\0'`; it defaults to `str32`.

## `n t`
The static version of the dynamic string type, `t`, with a max of `n` items.

## `'...'`
A dynamic string that doesn't support interpolation.

## `"..."`
A dynamic string that supports interpolation.

## `n '...'` or `n "..."`
A static `str32` of a max of `n` characters, containing `...`, with the rest, if any, being zero`d out.

## `n t '...'` or `n t "..."` or `t n '...'` or `t n "..."`
A static string of type `t`, of a max of `n` characters, containing `...`, with the rest, if any, being zero`d out.

## `static '...'` or `static "..."`
A static `str32`; the number of characters in `...` is its max.

## `static t '...'` or `static t "..."`
A static string of type `t`.

## `"$name"`, `"$$identifier_name"`, `"$@property_name"`, `"$&attribute_name"`, `"$(expression)"`
String interpolation.

## Escape Sequences
* `\\` — `\`
* `\'` — `'`
* `\"` — `"`
* `\u`*`hh`* — the unicode character with the hexadecimal code *`hh`*
* `\u(`*`...`*`)` — the unicode character with the code from the number literal *`...`*
* `\ub(`*`...`*`)` — the unicode character with the code from the binary literal *`...`*
* `\uo(`*`...`*`)` — the unicode character with the code from the octal *`...`*
* `\ux(`*`...`*`)` — the unicode character with the code from the hexadecimal *`...`*
* `\0` — `NUL`
* `\h` — `SOH`
* `\x` — `STX`
* `\X` — `ETX`
* `\T` — `EOT`
* `\q` — `ENQ`
* `\k` — `ACK`
* `\a` — `BEL`
* `\b` — `BS`
* `\t` — `TAB`
* `\n` — `LF`
* `\v` — `VT`
* `\f` — `FF`
* `\r` — `CR`
* `\o` — `SO`
* `\i` — `SI`
* `\l` — `DLE`
* `\1` — `DC1`
* `\2` — `DC2`
* `\3` — `DC3`
* `\4` — `DC4`
* `\K` — `NAK`
* `\s` — `SYN`
* `\B` — `ETB`
* `\c` — `CAN`
* `\m` — `EM`
* `\S` — `SUB`
* `\e` — `ESC`
* `\F` — `FS`
* `\G` — `GS`
* `\R` — `RS`
* `\U` — `US`
* `\d` — `DEL`

##  `#s`
The length of `s`: the number of unicode characters in it.

## `s#i`
A string containing the character in `s` at `i`, or `#s + i` if `i` is negative.

## `s##i`
The code of the character in `s` at `i`—or `#s + i` if `i` is negative—as an unsigned integer.

## `s#a_range`
A slice of `s`.

## `s##a_range`
An unsigned integer array of the codes of the characters in `s#a_range`.

## `s at substring`
An array containing all indices of `substring` in `s`. `substring` can be a pattern (see [Patterns](#patterns) for more details).

## `s at substring = new_substring`
A copy of `s` where all occurences of `substring` are replaced with `new_substring`. `substring` can be a pattern (see [Patterns](#patterns) for more details).

## `s1 s2`
A string resulting from the concatenation of `s1` and `s2` respectively.

## `s1..s2`
A string resulting from the concatenation of `s1` and `s2` respectively, with the character range, from the last character in `s1` to the first one in `s2`, inserted in-between.

## `s <- new_substring`
A `copy` of `s` with each character in `new_substring` inserted after it.

## `s#i <- new_substring`
A `copy` of `s` with each character in `new_substring` inserted after `copy#i`.

## `s#a_range <<- new_substring`
Insert each character in `new_substring` in the boundary of `s#a_range`.

## `s#i = x`
Set `s#i` to `x`.

## `s#a_range = x`
Set `s#a_range` to `x`.

## `s where routine`
An string where `routine` returns `true` for all characters in `s`. `routine` takes an item and an index respectively.

## `s via routine`
A copy of `s` where `routine` is applied to all characters. `routine` takes an item and an index respectively.

## `s via dictionary`
```
dictionary per k of v
	s#k = v
```

## `s down routine`
Start-to-end string reduction.

## `s up routine`
End-to-start string reduction.

## `sort s by routine`
A copy of `s` sorted by `routine`.

## `reverse s`
A reversed copy of `s`.

## `lower s`
A full-lowercase copy of `s`.

## `upper s`
An full-uppercase copy of `s`.

## `flip s`
A copy of `s` where all lowercase characters are converted to uppercase, and vice versa.

## `capital s`
A title-cased copy of `s`.

## `s in encoding_name`
An encoded copy of `s` in the encoding named, `encoding_name`.

## `isalpha s`
Whether all characters in `s` are alphabetic, or `false` if `s` is empty.

## `isalnum s`
Whether all characters in `s` are alphanumeric, or `false` if `s` is empty.

## `isascii s`
Whether all characters in `s` are ASCII, or `false` if `s` is empty.

## `isdecimal s`
Whether all characters in `s` are decimal, or `false` if `s` is empty.

## `isnumeric s`
Whether all characters in `s` are numeric, or `false` if `s` is empty.

## `isname s`
Whether `s` in a syntactic name, or `false` if `s` is empty.

## `istitle s`
Whether `s` is in title-case, or `false` if `s` is empty.

## `islower s`
Whether all characters in `s` are lowercase, or `false` if `s` is empty.

## `isupper s`
Whether all characters in `s` are uppercase, or `false` if `s` is empty.

## `isprindictionary s`
Whether all characters in `s` are prindictionary, or `false` if `s` is empty.

## `isspace s`
Whether all characters in `s` are whitespace, or `false` if `s` is empty.

## `split s with separator`
An array containing all the subtrings in `s` separated by `separator`, which can be a pattern (see [Patterns](#patterns)).

## `split s`
`split s with ',' ' '+` (see [Patterns](#patterns)).

## `trim s`
`s` with no whitespace at the start and end.

## `starttrim s`
`s` with no whitespace at the start.

## `endtrim s`
`s` with no whitespace at the end.

# Patterns

Patterns are like regular expressions. A string can substitute a pattern in any expression. Word characters are characters that could be part of a word—in any language—plus the underscore. Word boundaries seperate non-word from word characters. Non-word boundaries seperate non-word from non-word characters, or vice versa.

## `pat`
The pattern type.

## `.`
A pattern matching any unicode character.

## `start`
A pattern matching the start of the matched object.

## `end`
A pattern matching the end of the matched object.

## `-`
A pattern matching a word boundary.

## `~`
A pattern matching a non-word boundary.

## `p*`
A pattern matching zero or more occurences of `p`.

## `p**`
The greedy version of `p*`.

## `p+`
A pattern matching one or more occurences of `p`.

## `p++`
The greedy version of `p+`.

## `p n`
A pattern matching `n` occurences of `p`.

## `p a_range`
A pattern matching `a_range` occurences of `p`.

## `p?`
A pattern matching `p` or nothing.

## `p??`
The greedy version of `p?`.

## `!p`
A pattern matching anything but `p`.

## `p1 p2`
A pattern matching `p1` then `p2`.

## `p1 | p2`
A pattern matching `p1` or `p2`.

## `(p)`
A pattern grouping `p`.

## `[p]`
A captured pattern.

## `x^[p]`
A captured pattern named `x`.

## `^n`
The `n`th captured pattern.

## `^x`
The captured pattern named `x`.

# Formats

## `fmt`
The format type.

## ``` `...{x}...` ```
A format from a literal; `x` is a name.

TODO

# Enumerators & Enumerals

Enumerals are user-defined multary versions of booleans. Enumerators are the types of identifiers to which enumerals are assigned. The first enumeral of an enumerator is equal (not by identity) to `1`.

## `enum`
The enumerator type.

## `enumeral`
The enumeral type.

## `enum e x, y, etc`
An enumerator named, `e`, with enumerals: `x`, `y`, etc.

## `e.x` or `x` (if not overridden)
`e`'s enumeral, `x`.

# Bit Fields

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

# Versions

Specifically, semantic versions. Version parts can be integers, names or strings; use `(x)` to put the value of `x` in place of a part.

## `x.y.z`
A version with the major part, `x`, the minor part, `y`, and the patch, `z`.

## `x.y.z-a.b.etc`
A version with the major part, `x`, the minor part, `y`, the patch, `z`, and the pre-release, `a.b.etc`.

## `x.y.z+e.f.etc`
A version with the major part, `x`, the minor part, `y`, the patch, `z`, and the metadata part, `e.f.etc`.

## `x.y.z-a.b.etc+e.f.etc`
A version with the major part, `x`, the minor part, `y`, the patch, `z`, the pre-release, `a.b.etc`, and the metadata part, `e.f.etc`.

##  `major v`
The major part of the version, `v`, as a `nat`.

##  `minor v`
The minor part of the version, `v`, as a `nat`.

##  `patchof v`
The patch of the version, `v`, as a `nat`.

# Memory Blocks

## `mem`
The memory block type.

## `%[x#y]`
A memory block from the address `x`.

## `%[#y]`
A newly allocated memory block of `y` bytes.

## `%[x]`
A newly allocated memory block of just enough size for `x`, with `x` written to it.

## `#memory_block`
The size of `memory_block` in bytes.

## `memory_block = x`
Write `x` to `memory_block`, and return `memory_block`.

## `delete memory_block`
Free the memory block represented by `memory_block`. Note that internally allocated memory blocks are automatically freed when garbage-collected.

# Paths

Path components (e.g. `x` in `/x/y`) are literal; use `(x)` to put `x`'s value as a string, in place of the component. `..` as a component refers to the parent directory of the preceding one.

## `path`
The path type.

## `./x/y/etc` or `../x/y/etc`
A relative local path.

## `/x/y/etc`
An absolute local path.

## `d:/x/y/etc`
An absolute local Windows path under the `d` drive; `d` is case-insensitive.

## `protocol://userinfo@host:port/x/y/etc?a=b&c=etc#fragment`
A remote path; each one of `userinfo@`, `:port`, `/x/y/etc`, `?a=b&c=etc` and `#fragment` is omitdictionary.

## `p#i`
The `i`th component of the path, `p`.

## `str path`
The content of the file/socket at `path`.

## `pathsep`
The local platform's file path separator.

# Files

The supported file encodings out of the box are `latin1`, `utf8`, `utf16` and `utf32`.

## `file`
The file type.

## `here`
The current working directory.

## `top`
The parent of the current working directory.

## `root`
The root directory.

## `home`
The home directory.

## `file encoding path`
A file at `path`, encoded in `encoding`.

## `file path`
`file utf8 path`.

## `f#i`
The `i`th character in `f`.

## `f#a_range`
A string slice of `f`.

## `f path`
Reopen `f` with `path`.

## `close f`
Close the file `f`. Note that files are automatically closed when garbage-collected.

## `f = x`
Overwrite 'f' with `x`.

## `f <- x`
Write `x` to the end of `f`.

## `f#i <- x`
Write `x` after `f#i`.

## `f#a_range <<- x`
Insert each character in stringified `x`, in the boundary of `f#a_range`.

## `str f`
A string containing all characters in `f`.

## `stream f`
A stream of all characters in `f` (see [Streams](#streams)).

## `f.x`
The file named, `x`, inside the directory `f`; `x` can be a name or string.

## `top f`
The parent directory of `f`.

## `delete f`
Delete `f`.

## `trash f`
Move `f` to the trash.

## `move f to d`
Move `f` to the directory, `d`.

## `copy f to d`
Copy `f` to the directory, `d`.

## `move f1 to f2`
Move `f1` to `f2`.

## `copy f1 to f2`
Copy `f1` to `f2`.

## `rename f to name`
Rename `f` to `name`.

# Stdout, Stdin & Stderr

## `write x`
Write `x` to stdout.

## `rewrite x`
Write `'\r'..x` to stdout.

## `print x`
Write `x..'\n'` to stdout.

## `reprint x`
Write `'\r'..x..'\n'` to stdout.

## `error x`
Write `x` to stderr.

## `reerror x`
Write `'\r'..x` to stderr.

## `printerror x`
Write `x..'\n'` to stderr.

## `reprinterror x`
Write `'\r'..x..'\n'` to stderr.

## `input`
A line from the standard input, without the newline.

# Streams

## `t...`
The type of streams yielding objects of type `t`.

## `stream collection`
A stream of `collection`.

## `stream synchronous_routine_definition`
A stream from a routine: a generator. `yield x` inside `synchronous_routine_definition` yields `x`.

## `nextin s`
The next item from `s`.

## `next n s`
An array of the next `n` items from `s`.

## `collection per item_name block`
If `collection` is mudictionary: new collection of the same type, with `block` as an item for each item in `collection`; otherwise: evaluate `block` for each `nextin collection`.

## `collection per index_name of item_name block`
If `collection` is mudictionary: new collection of the same type, with `block` as an item and `index_name` as a key for each item in `collection`; otherwise: evaluate `block` for each `nextin collection`.

# Sockets

The supported network protocols out of the box are `ipv4`, `ipv6`...

## `socket`
The socket type.

## `socket path procedure`
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

# IPv4 Packets

IPv4 packets and IP options are mudictionary.

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
`p`'s protocol; can be `ICMP`, `IGMP`, `TCP`, `UDP`, `ENCAP`, `OSPTF` or `SCTP`, which are of type `ipprotocol` (see [Enumerators & Enumerals](#enumerators--enumerals)).

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
`o`'s type; can only be `EOOL`, `NOP`, `SEC`, `RR`, `ZSU`, `MTUP`, `MTUR`, `ENCODE`, `QS`, `EXP`, `TS`, `TR`, `EXP`, `SEC`, `LSR`, `E-SEC`, `CIPSO`, `SID`, `SSR`, `VISA`, `IMITD`, `EIP`, `ADDEXT`, `RTRALT`, `SDB`, `DPS`, `UMP`, `EXP`, `FINN` or `EXP`, which are of type `ipopttype` (see [Enumerators & Enumerals](#enumerators--enumerals)).

## `o.data`
`o`'s data.

# IPv4 Addresses

## `ipv4addr`
The IPv4 address type.

## `ipv4addr c`
An IPv4 address from the collection, `c`.

## `a#i`
The `i`th of 4 divided numbers of the address, `a`.

## `a#a_range`
An array of the divided numbers of `a` in the range, `a_range`.

## `a#i = x`
Set `a#i` to `x`.

## `a#a_range = x`
Set `a#a_range` to the array, `x`.

# IPv6 Packets

IPv6 packets are mudictionary.

## `ipv6packet`
The IPv6 packet type.

## `ipv6packet c`
An IPv6 packet from the collection, `c`.

## `p.class`
`p`'s traffic class.

## `p.label`
`p`'s flow label.

## `p.payload`
`p`'s payload.

## `#p.payload`
`p`'s payload length in bytes.

## `p.nextheader`
`p`'s Next Header.

## `p.hoplimit`
`p`'s hop limit.

## `p.srcaddr`
`p`'s source address.

## `p.destaddr`
`p`'s destination address.

## `p.payload`
`p`'s payload.

# IPv6 Addresses

## `ipv6addr`
The IPv6 address type.

## `ipv6addr c`
An IPv6 address from the collection, `c`.

## `a#i`
The `i`th of 4 divided numbers of the address, `a`.

## `a#a_range`
An array of the divided numbers of `a` in the range, `a_range`.

## `a#i = x`
Set `a#i` to `x`.

## `a#a_range = x`
Set `a#a_range` to the array, `x`.

# ICMP Packets

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

# ICMPv6 Packets

## `icmpv6packet`
The ICMPv packet type.
6
## `icmpv6packet c`
An ICMPv6 packet from the collection, `c`.

## `p.type`
`p`'s type.

## `p.code`
`p`'s code.

## `p.checksum`
`p`'s checksum.

## `p.body`
`p`'s message body.

## `p.mtu`
`p`'s MTU; available for some packet types and codes.

## `p.pointer`
`p`'s pointer; available for some packet types and codes.

## `p.id`
`p`'s identifier; available for some packet types and codes.

## `p.seqnumber`
`p`'s sequence number; available for some packet types and codes.

## `p.data`
`p`'s data; available for some packet types and codes.

## `p.options`
`p`'s options; available for some packet types and codes.

## `p.hoplimit`
`p`'s current hop limit; available for some packet types and codes.

## `p.addrconf`
Whether `p`'s managed address configuration flag is set; available for some packet types and codes.

## `p.otherconf`
Whether `p`'s other configuration flag is set; available for some packet types and codes.

## `p.rlifetime`
`p`'s router lifetime; available for some packet types and codes.

## `p.reachtime`
`p`'s reachable time; available for some packet types and codes.

## `p.retranstimer`
`p`'s retrans timer; available for some packet types and codes.

## `p.targetaddr`
`p`'s target address; available for some packet types and codes.

## `p.destaddr`
`p`'s destination address; available for some packet types and codes.

## `p.override`
Whether `p`'s override flag is set; available for some packet types and codes.

## `p.solicited`
Whether `p`'s solicited flag is set; available for some packet types and codes.

## `p.router`
Whether `p`'s router flag is set; available for some packet types and codes.

TODO: research this shit above and continue networking stuff

# Times

All time properties start at `0`.

## `time`
The time type.

## `now`
Now.

## `t.ns`
The nanosecond of `t`.

## `t.ms`
The millisecond of `t`.

## `t.s`
The second of `t`.

## `t.m`
The minute of `t`.

## `t.H`
The 24-hour of `t`.

## `t.h`
The 12-hour of `t`.

## `t.phase`
The phase of `t`: either `AM` or `PM` (see [Enumerators & Enumerals](#enumerators--enumerals)).

## `t.wkd`
The week day of `t`.

## `t.d`
The month day of `t`.

## `t.yd`
The year day of `t`.

## `t.wk`
The month week of `t`.

## `t.ywk`
The year week of `t`.

## `t.mo`
The month of `t`.

## `t.Y`
The year of `t`.

## `t.y`
The number with the first two digits of the year of `t`.

## `x - y`
The difference, in milliseconds, between the times: `x` and `y`; it can be negative.

## `t as f`
`t` formatted with the format, `f`.

## `time c`
A time from the collection, `c`.

# Progresses

## `progress`
The progress type, or a progress with the default format.

## `progress f`
A progress with the format, `f`: TODO

## `p` as `bool`
Whether the progress, `p`, is ongoing.

## `p x outof y`
Start `p` with a total of `x`, and a current value of `y`.

## `p at n`
Set `p`'s current value to `n`.

## `p x`
`p 0 outof x`.

# Exceptions

## `exception type_parameters`
The type of exceptions that take `type_parameters`, which only contains types, and return a object of type `t`.

## `exception e parameters x`
The definitions of an exception that takes `parameters` and returns the string, `x`.

## `throw e arguments`
Throw `e`.

## `try expression except parameters expression`
Evaluate `expression`; if it throws exceptions, catch it and pass them to parameters and evaluate `expression`.

## `expression except parameters expression`
`try expression except parameters expression`.

## `try expression`
Evaluate `expression` and catch any exceptions it throws.

# Routines

Parameters are omitdictionary except in some obvious cases. Routines that return `null` are called, procedures.

## `type_parameters -> t`
The type of synchronous routines that take `type_parameters`, which only contains types, and return a object of type `t`.

## `type_parameters -|`
`type_parameters -> null`.

## `async type_parameters -> t`
The type of asynchronous routines that take `type_parameters`, which only contains types, and return a object of type `t`.

## `async type_parameters -|`
`async type_parameters -> null`.

## `parameters -> expression`
A synchronous routine that takes `parameters`, and returns `expression`.

## `parameters -|`
`parameters -> null`.

## `async parameters -> expression`
An asynchronous routine that takes `parameters`, and returns `expression`.

## `async parameters -|`
`async parameters -> null`.

## Parameters
Parameters can be:
* `x` — a single regular parameter
* `(x, y, etc)` — regular parameters
* `<t, u, etc>` — generic parameters
* `<t, u, etc> (x, y, etc)` — generic and regular parameters
* `parameters: t` — parameters with a specified return value type—not valid in a routine type expression.

Special parameter syntax:

* `x: t` — a required parameter of type `t`
* `x: t?` — an optional parameter of type `t`, with a variable position
* `x = y` — an optional parameter with a constant position, that's assigned `y` if not given
* `x: t = y` — an optional parameter of type `t`, with a constant position, that's assigned `y` if not given
* `p1 | p2 | etc` — a parameter disjunction where the parameters share the same position; they must have different types from each others'
* `copy p` — makes `p`'s argument get copied before getting passed.

## `f` or `f()`
Call `f` with no arguments.

## `(f)`
Return `f` instead of calling it.

## `f(x, y=z, etc)`
Call `f` with the argument, `x`, passed to the first parameter, and the argument, `z`, passed  to the parameter with the name, `y`, and return its return value. The parentheses can be omitted for single arguments.

## `call!`
Block the process until `call` returns a value, then return that.

## `#n`
The `n`th function argument—inside functions, or the `n`th command line argument—inside the global scope; command line arguments are processed (also see [.x](#x-5)).

## `.x`
The function argument whose parameter is named, `x`—inside functions, or the command line argument whose parameter is named, `x`—inside the global scope.

## `return x`
Return `x`.

## `f parameters = expression`
`f = parameters -> expression`

## `async f parameters = expression`
`f = async parameters -> expression`

## `f parameters block`
`f = parameters -> (block)` (see [Blocks](#blocks)).

## `async f parameters block`
`f = async parameters -> (block)`.

# Classes

Classes are user-defined types. Class parameters or constructor parameters follow the same rules of routine parameters.

## `the c parameters expression`
A class named, `c`, whose constructor takes `parameters`, and evaluates `expression` in its scope.

## `default c`
`c`'s default value identifier (see [Identifiers](#identifiers)); when assigned (`default c = x`), declared identifiers of type `c` are automatically assigned it.

## Class Parameters
Class parameters look like `@x` or `&x` where `x` is the name of the parameter and property/attribute to be assigned whatever argument is passed to the parameter, when the class is instanciated.

## `this`
The instance; accessable inside a class' scope.

## `@x`
The property named, `x`; accessable inside a class' scope.

## `&x`
The attribute named, `x`; accessable inside a class' scope.

## `c arguments`
A new instance of `c`.

## `i.x`
The property, `x`, of the instance, `i`.

## `c.x`
The attribute, `x`, of the class, `c`.

## Inheritance
Inhertitance can be achieved by expanding an instance of the superclass inside the subclass, like:

```
the subclass parameters
	* superclass arguments
```

# Identifiers

Objects are automatically converted to identifiers where identifiers are expected: `'...' = x`.

## `id`
The identifier type.

## `%i`
A first-class identifier named, `i`.

## `$i`
The value referred to by the identifier, `i`.

## `i: t`
An identifier named, `i`, that only refer to objects of type `t`. If not defined (only declared), it is zero'd out, or assigned `t`'s default value.

## `i = x`
An identifier named, `i`, referring to `x`.

## `const i = x` or `const i: t = x`
An identifier named, `i`, that can't be reassigned.

## `=x`
`x = x`.

## `o=x`
`x o= x` where `o` is an operator.

# Control Flow

See [Streams](#streams) for for-in loop syntax. All loops return an array of evaluated `block`s in each iteration.

## `if x block`
If `x` is true, evaluate `block`. This is always a statement.

## `unless x block`
`if (not x) block`.

## `if x block else y`
Evaluate `block` if `x` is true; `y` otherwise.

## `unless x block else y`
`if (not x) block else y`

## `case o x => y z block`
If `o == x`, return `y`; otherwise, if `o == z`, return `block`. Pattern matching is supported.

## `while x block`
While `x` is true, evaluate `block`.

## `until x block`
`while (not x) block`.

## `forever block`
`while true block`.

## `whenever x block`
`forever if x block`.

## `do x` or `block`
Evaluate `x` or `block` inside a subscope.

## `n timesdo x`
Evaluate `x`, `n` times.

## `out`
Break out of the current loop.

## `again`
Skip to the next iteration of the current loop.

## `x if y`
`x` if `y` is true. This is always a statement.

## `x if y else z`
`x` if `y` is true; `z` otherwise.

## `x unless y else z`
`x if not y else z`.

## `x else y`
`x` if it is true; `y` otherwise.

## `x while y`
An array, adding `x` to itself while `y` is true.

## `x unless y`
`x while not y`.

## `x forever`
`forever do x`.

## `x whenever y`
`whenever y do x`.

# Blocks

Blocks, are groups of expressions where the last expression is returned; they must be indented by the same amount of the same whitespace character: either spaces or tabs. `do expression` can be used in place of blocks.

## Example
`if` expression with a block expression:

```
if x
	expression1
	expression2
	etc
```

# Conversions

## `x as t` or `t x` (for some types)
A copy of the object/type, `x`, converted/adapted to the type `t`.

# Falsy Objects

* `null`
* `0`
* `false`
* empty collections

# External Code

No user operation is needed to import compiler-reachable code returning a `mod`. In that case, the compiler makes it available as a `mod` referred to by an identifier with the same filename, without `.i`; this is called autoporting.

## `path`
Include source code from the file/socket at `path`, at compile time.

# Modules

## `mod`
The module type.

## `mod expression`
A module where `expression` is evaluated inside its scope.

## `m.x`
The object named, `x`, inside the module, `m`.

# Miscellaneous

## `it`
Expands to the identifier being assigned.

## `in x block`
Evaluate `block` as if all keys in `x` are part of the current namespace.

## `copy x`
A copy of `x`.

## `env x`
The value of the environmental variable, `x`.

## `accept parameters`
Process command line arguments through `parameters` into the current namespace.

## `base i`
Set the index base to the positive integer, `i`, in the current scope.

## `async expression`
Evaluate `expression` asynchronously.

## `exit code`
Exit the process with `code`.

## `exit`
`exit 0`.

## `x o= y`
`x = x o y` where `o` is a binary operator.

## `x++`
`x += 1`.

## `x--`
`x -= 1`.

## `e block` where `e` expects a collection
`e c` where `c` is the collection containing each line in `block` as an item.

## `#t`
The size of instances of type `t`, in bytes.

TODO (high priority to low):
* TODOs
* images, videos, audio, etc
* graphics
* sound
* peripherals, bluetooth, wifi...
MAYBE:
* linked lists
* document the return types of everything
* examples
* italicize the stuff
