## `mem`
The memory block type.

## `%[x#y]`
A memory block from the address `x`.

## `%[#y]`
A newly allocated memory block of `y` bytes.

## `%[x]`
A newly allocated memory block of just enough size for `x`, with `x` written to it.

## `#memory_block`
The size of `memory_block` in bytes.

## `memory_block = x`
Write `x` to `memory_block`, and return `memory_block`.

## `delete memory_block`
Free the memory block represented by `memory_block`. Note that internally allocated memory blocks are automatically freed when garbage-collected.