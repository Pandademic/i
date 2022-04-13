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
Set the index base to the non-negative integer, `i`, in the current scope.

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