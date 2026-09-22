# Let polymorphism

↑ **Parent:** [Hindley-Milner type system](hindley-milner-type-system.md)

[Let polymorphism](let-polymorphism.md) gives an eligible `let`-bound name a [type scheme](type-scheme.md), allowing fresh instantiation at each use. In the pure [Hindley-Milner type system](hindley-milner-type-system.md), generalize the inferred type's [type variables](type-variable.md) that are free in that type and not free in the current [typing context](typing-context.md). The [identity function](identity-function.md) example under [type variable](type-variable.md) meets this condition. A [lambda abstraction](lambda-abstraction.md)'s parameter receives one monomorphic type shared by its uses. Languages with mutation, such as [Standard ML](standard-ml.md) with [ML reference types](ml-reference-type.md), need additional restrictions on generalization.

## ↑ Ancestors (5)

1. [Hindley-Milner type system](hindley-milner-type-system.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Hindley-Milner type system](hindley-milner-type-system.md)
- [Let polymorphism](let-polymorphism.md)
- [Type variable](type-variable.md)
- [Typing context](typing-context.md)
