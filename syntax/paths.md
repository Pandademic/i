Path components (e.g. `x` in `/x/y`) are literal; use `(x)` to put `x`'s value as a string, in place of the component. `..` as a component refers to the parent directory of the preceding one.

## `path`
The path type.

## `./x/y/etc` or `../x/y/etc`
A relative local path.

## `/x/y/etc`
An absolute local path.

## `d:/x/y/etc`
An absolute local Windows path under the `d` drive; `d` is case-insensitive.

## `protocol://userinfo@host:port/x/y/etc?a=b&c=etc#fragment`
A remote path; each one of `userinfo@`, `:port`, `/x/y/etc`, `?a=b&c=etc` and `#fragment` is omitdictionary.

## `p#i`
The `i`th component of the path, `p`.

## `str path`
The content of the file/socket at `path`.

## `pathsep`
The local platform's file path separator.