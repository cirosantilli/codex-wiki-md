# Type unification

↑ **Parent:** [Type inference](type-inference.md)

[Type unification](type-unification.md) finds a [type substitution](type-substitution.md) making specified type expressions equal, or reports incompatible constraints. In our [simple type](simple-type.md) grammar, matching two [function types](function-type.md) reduces to matching their argument types and their result types. Distinct base types `int` and `bool` fail to match; solving a [type variable](type-variable.md) against a nontrivial type expression uses the [occurs check](occurs-check.md).

// Target: computer-science.bigb

## ↑ Ancestors (5)

1. [Type inference](type-inference.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Algorithm W](algorithm-w.md)
- [Hindley-Milner type system](hindley-milner-type-system.md)
- [Occurs check](occurs-check.md)
- [Type inference](type-inference.md)
- [Type unification](type-unification.md)
