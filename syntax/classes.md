Classes are user-defined types. Class parameters or constructor parameters follow the same rules of routine parameters.

## `the c parameters expression`
A class named, `c`, whose constructor takes `parameters`, and evaluates `expression` in its scope.

## `default c`
`c`'s default value identifier (see [Identifiers](#identifiers)); when assigned (`default c = x`), declared identifiers of type `c` are automatically assigned it.

## Class Parameters
Class parameters look like `@x` or `&x` where `x` is the name of the parameter and property/attribute to be assigned whatever argument is passed to the parameter, when the class is instanciated.

## `this`
The instance; accessable inside a class' scope.

## `@x`
The property named, `x`; accessable inside a class' scope.

## `&x`
The attribute named, `x`; accessable inside a class' scope.

## `c arguments`
A new instance of `c`.

## `i.x`
The property, `x`, of the instance, `i`.

## `c.x`
The attribute, `x`, of the class, `c`.

## Inheritance
Inhertitance can be achieved by expanding an instance of the superclass inside the subclass, like:

```
the subclass parameters
	* superclass arguments
```