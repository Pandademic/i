The built-in collections are arrays, ranges, tuples, sets, dictionaries, matrices, strings, paths, files, streams and classes. All of them are iterable (see streams).

Doing a scalar operation on an array, tuple, dictionary or matrix, with scalar items result in a new one where the operation is done on all items.

Empty collections are falsy.

## `concat c with sep`
A string containing the stringified versions of all items from collection `c` in order, separated with separator `sep`, which can be a pattern.

See *patterns.md*.

## `concat c`
`concat c with ''`.

## `comma c`
`concat c with ', '`.

## `* c`
Syntactically expand collection `c`.