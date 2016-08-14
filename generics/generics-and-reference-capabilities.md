# Generics and Reference Capabilities

In the examples presented previously we've explicitly set the reference capability to `val`:

    class Foo[A: Any val]

If the capability is left out of the type parameter then the generic class or function can accept any reference capability. This would look like:

    class Foo[A: Any]

It can be made shorter because `Any` is the default constraint, leaving us with:

    class Foo[A]

This is what the example shown before looks like but with any reference capability accepted:


