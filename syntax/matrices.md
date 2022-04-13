Matrices are static. The mathematical operations here can only work on number matrices. Matrices whose rows only contain one item each are called vectors.

## `n [;t]` or `n [t;]`
The type of matrices of a max of `n` items of type `t`.

## `n [;]`
An empty matrix with a context-dependent type.

## `t n [;]`
An empty matrix that can contain items of type `t`.

## `[a11, a12, etc; a21, a22, etc; etc]`
A matrix; the number of items in `a11, a12, etc; a21, a22, etc; etc` is its max.

## `n [a11, a12, etc; a21, a22, etc; etc]`
A matrix of a max of `n` items.

## `t n [a11, a12, etc; a21, a22, etc; etc]`
A dynamic matrix of a max of `n` items of type `t`.

## `[;x]` or `[x;]`
A matrix with one item, `x`.

## `[x; y; z]`
A vector.

## `#m`
The number of items in `m`.

## `m#i`
If `i` is a terminal index: an item in `m`; otherwise a submatrix of `m`.

## `m#(i, j, etc)`
If `(i, j, etc)` is a terminal index: an item in `m`; otherwise a submatrix of `m`.

## `m#(i, j, etc) = x`
Set `m#(i, j, etc)` to `x`.

## `transpose m`
A transposed copy of `m`.

## `m1 * m2` or `m1 m2`
Matrix multiplication.

## `[a11, a12, etc; a21, a22, etc; etc] = m`
Vector destructuring: `a11, a12 = m#1`, `a21, a22 = m#2`, etc.

## `v.x`, `v.s` or `v.r`
`v#1` where `v` is a vector.

## `v.y`, `v.t` or `v.g`
`v#2`.

## `v.z`, `v.u` or `v.b`
`v#3`.

## `v.w`, `v.v` or `v.a`
`v#4`.

## `|v|`
The magnitude of `v`.

## `norm v`
A normalized copy of `v`.

## `v1 dot v2`
The dot product of `v1` and `v2`.

## `v1 cross v2`
The cross product of `v1` and `v2`.

## `v1 theta v2`
The angle between `v1` and `v2`.

## `[x; y; etc] = v`
Vector destructuring: `x = v#x`, `y = v#y`, etc.