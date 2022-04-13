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