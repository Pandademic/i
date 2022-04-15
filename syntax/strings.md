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

## `'...'B` or `"..."B`
`'...'` as a `u8` array.

## `'...'b` or `"..."b`
`'...'` as an `i8` array.

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