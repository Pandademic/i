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

See *functions.md/Parameters*.

## `tobase1` (or somethin')
Set the index base to `1` in the current scope.

## `async x`
Evaluate expression `x` asynchronously.

## `exit n`
Exit the process with code `n`.

## `exit`
Exit the process with code `0`.

## `x op= y`
`x = x op y` where `o` is a binary operator that isn't `=`.

## `x++`
`x += 1`.

## `x--`
`x -= 1`.

## `x block` where `x` expects a collection
`x c` where `c` is the collection containing each line in `block` as an item.

## `#T`
The size of instances of type `T`, in bytes.