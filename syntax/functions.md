Functions are overloadable. Parameters are omittable except in some obvious cases.

## `type_parameters => t`
The type of synchronous functions that take `type_parameters`, which only contains types, and return a object of type `t`.

## `type_parameters =|`
`type_parameters => null`.

## `async type_parameters => t`
The type of asynchronous functions that take `type_parameters`, which only contains types, and return a object of type `t`.

## `async type_parameters =|`
`async type_parameters => null`.

## `parameters => expression`
A synchronous function that takes `parameters`, and returns `expression`.

## `parameters =|`
`parameters => null`.

## `async parameters => expression`
An asynchronous function that takes `parameters`, and returns `expression`.

## `async parameters =|`
`async parameters => null`.

## Parameters
Parameters can be:
* `x` — a single regular parameter
* `(x, y, etc)` — regular parameters
* `<t, u, etc>` — generic parameters
* `<t, u, etc> (x, y, etc)` — generic and regular parameters
* `parameters: t` — parameters with a specified return value type—not valid in a function type expression.

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

## `c args`
Call each function in function collection `c` with `args` (which can be `()`), and return a collection with the same type, containing the respective return values.

## `call!`
Block the process until `call` returns a value, then return that.

## `#n`
The `n`th function argument—inside functions, or the `n`th command line argument—inside the global scope; command line arguments are processed (also see [.x](#x-5)).

## `.x`
The function argument whose parameter is named, `x`—inside functions, or the command line argument whose parameter is named, `x`—inside the global scope.

## `return x`
Return `x`.

## `f parameters = expression`
`f = parameters => expression`

## `async f parameters = expression`
`f = async parameters => expression`

## `f parameters block`
`f = parameters => (block)` (see [Blocks](#blocks)).

## `async f parameters block`
`f = async parameters => (block)`.