No user operation is needed to import compiler-reachable code returning a `mod`. In that case, the compiler makes it available as a `mod` referred to by an identifier with the same filename, without `.i`; this is called autoporting.

## `path`
Include source code from the file/socket at `path`, at compile time.