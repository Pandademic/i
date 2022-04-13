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