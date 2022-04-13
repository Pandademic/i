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