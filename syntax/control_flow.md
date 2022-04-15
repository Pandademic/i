See *streams.md* for for-in loop syntax. All expression loops return an array of evaluated blocks in each iteration. Also, see *blocks.md*.

## `if x block` or `y if x`
If `x` is true, evaluate `block`/`y`. This is always a statement.

## `unless x block` or `y unless x`
If `x` is false, evaluate `block`/`y`. This is always a statement.

## `if x block else z` or `y if x else z`
Return `block`/`y` if `x` is true. `z` otherwise.

## `unless x block else y` or `y unless x else z`
Return `block`/`y` if `x` is false. `z` otherwise.

## `case x x1 y1 x2 y2 ...`
A switch statement/expression. If `x == x1`, return `y1`. otherwise, if `x == x2`, return `y2`. And so on. If `x1`, `x2`, etc are patterns, pattern matching happens. Enclosing them in parentheses, treats them as regular values.

## `while x block` or `y while x`
While `x` is true, evaluate `block`/`y`.

## `until x block` or `y until x`
While `x` is false, evaluate `block`/`y`.

## `forever block` or `x forever`
Keep evaluating `block`/`x`.

## `whenever x block` or `y whenever x`
Keep checking if `x` is true, and evaluate `block`/`y` whenever it is.

Equivalent to `forever if x block`.

## `do x` or `block`
Evaluate `x` or `block` inside a subscope.

## `n timesdo x`
Evaluate `x`, `n` times.

## `out`
Break out of the current loop.

## `again`
Skip to the current iteration of the current loop.