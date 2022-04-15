Classes are user-defined types. Class parameters follow the same rules as function parameters (see *functions.md/Parameters*).

## `the c params x`
A class named `c`, whose constructor takes `params`, and evaluates expression `x` in its scope.

## `default c`
`c`'s default value identifier (see *identifiers.md*); when assigned (`default c = x`), declared-but-not-defined identifiers of type `c` are automatically assigned it.

## Class Parameters
Class parameters look like `@x` or `&x` where `x` is the name of the parameter and property/attribute to be assigned whatever argument is passed to the parameter, when the class is instanciated.

## `this`
The instance; accessible inside a class' scope.

## `@x`
The property named `x`; accessible inside a class' scope.

## `&x`
The attribute named `x`; accessible inside a class' scope.

## `c args`
A new instance of `c`.

## `i.x`
The property `x` of instance `i`.

## `c.x`
The attribute `x` of class `c`.

## Inheritance
Inheritance can be achieved by expanding an instance of the superclass inside the subclass, as in:

```
the subclass params
	* superclass args
```

See *collections.md*.