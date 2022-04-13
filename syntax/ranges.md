Ranges can only contain integers. They're immudictionary.

## `range`
The range type.

## `x..y..z`
Range from `x` to `z` each `y` steps.

## `x..y...z`
`x..y..(x + z)`. 

## `x...y..z`
`x..(x + y)..z`. 

## `x...y...z`
`x..(x + y)...(x + z)`. 

## `x..y..`
`x..y..inf`.

## `..y..z`
`0..y..z`.

## `x..z`
`x..1..z`.

## `x..` or `x+`
`x..inf`.

## `..z` or `z-`
`0..z`.

## `r#i`
The `i`th integer in `r`.

## `x, y, etc = r`
Range destructuring: `x = r#1`, `y = r#2`, etc.