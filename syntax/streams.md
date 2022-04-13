## `t...`
The type of streams yielding objects of type `t`.

## `stream collection`
A stream of `collection`.

## `stream synchronous_routine_definition`
A stream from a routine: a generator. `yield x` inside `synchronous_routine_definition` yields `x`.

## `nextin s`
The next item from `s`.

## `next n s`
An array of the next `n` items from `s`.

## `collection per item_name block`
If `collection` is mudictionary: new collection of the same type, with `block` as an item for each item in `collection`; otherwise: evaluate `block` for each `nextin collection`.

## `collection per index_name of item_name block`
If `collection` is mudictionary: new collection of the same type, with `block` as an item and `index_name` as a key for each item in `collection`; otherwise: evaluate `block` for each `nextin collection`.