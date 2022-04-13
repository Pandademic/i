Specifically, semantic versions. Version parts can be integers, names or strings; use `(x)` to put the value of `x` in place of a part.

## `x.y.z`
A version with the major part, `x`, the minor part, `y`, and the patch, `z`.

## `x.y.z-a.b.etc`
A version with the major part, `x`, the minor part, `y`, the patch, `z`, and the pre-release, `a.b.etc`.

## `x.y.z+e.f.etc`
A version with the major part, `x`, the minor part, `y`, the patch, `z`, and the metadata part, `e.f.etc`.

## `x.y.z-a.b.etc+e.f.etc`
A version with the major part, `x`, the minor part, `y`, the patch, `z`, the pre-release, `a.b.etc`, and the metadata part, `e.f.etc`.

##  `v.major`
The major part of the version, `v`, as a `nat`.

##  `v.minor`
The minor part of the version, `v`, as a `nat`.

##  `v.patch`
The patch of the version, `v`, as a `nat`.