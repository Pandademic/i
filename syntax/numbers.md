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

`0` is falsy.

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
A bit field from `x` in the boundary of `a_range` (see [Bit Fields](#bit-fields)).

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