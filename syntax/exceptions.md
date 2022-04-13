## `exception type_parameters`
The type of exceptions that take `type_parameters`, which only contains types, and return an object of type `t`.

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