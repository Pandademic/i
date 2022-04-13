The types of collections are [arrays](#arrays), [ranges](#ranges), [tuples](#tuples), [sets](#sets), [dictionaries](#dictionaries), [matrices](#matrices), [strings](#strings), [enumerators](#enumerators--enumerals), [bit fields](#bit-fields), [paths](#paths), [files](#files), [streams](#streams) and [classes](#classes). All of them are iterable (see [Streams](#streams)).

Doing a scalar operation on an array, tuple, dictionary, matrix or string, with scalar items result in a new one where the operation is done on all of its items.

Empty collections are falsy.

## `concat collection with separator`
A string containing the stringified versions of all items from `collection` in order, separated with `separator`, which can be a pattern (see [Patterns](#patterns)).

## `concat collection`
`concat collection with ''`.

## `comma collection`
`concat collection with ', '`.

## `* collection`
Syntactically expand `collection`.