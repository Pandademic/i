The supported file encodings out of the box are `latin1`, `utf8`, `utf16` and `utf32`.

## `file`
The file type.

## `here`
The current working directory.

## `top`
The parent of the current working directory.

## `root`
The root directory.

## `home`
The home directory.

## `file encoding path`
A file at `path`, encoded in `encoding`.

## `file path`
`file utf8 path`.

## `f#i`
The `i`th character in `f`.

## `f#a_range`
A string slice of `f`.

## `f path`
Reopen `f` with `path`.

## `close f`
Close the file `f`. Note that files are automatically closed when garbage-collected.

## `f = x`
Overwrite 'f' with `x`.

## `f <- x`
Write `x` to the end of `f`.

## `f#i <- x`
Write `x` after `f#i`.

## `f#a_range <<- x`
Insert each character in stringified `x`, in the boundary of `f#a_range`.

## `str f`
A string containing all characters in `f`.

## `stream f`
A stream of all characters in `f` (see [Streams](#streams)).

## `f.x`
The file named, `x`, inside the directory `f`; `x` can be a name or string.

## `top f`
The parent directory of `f`.

## `delete f`
Delete `f`.

## `trash f`
Move `f` to the trash.

## `move f to d`
Move `f` to the directory, `d`.

## `copy f to d`
Copy `f` to the directory, `d`.

## `move f1 to f2`
Move `f1` to `f2`.

## `copy f1 to f2`
Copy `f1` to `f2`.

## `rename f to name`
Rename `f` to `name`.