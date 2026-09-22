# Type inference

↑ **Parent:** [Type system](type-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_inference)

[Type inference](type-inference.md) discovers types consistent with a program's structure and [typing context](typing-context.md). In our examples, it introduces fresh [type variables](type-variable.md), generates [equations](equation.md) from [typing judgments](typing-judgment.md), and solves them by [type unification](type-unification.md). For $f\,3$, if $f$ initially has unknown type $\alpha$ and the result has fresh type $\beta$, [lambda application](lambda-application.md) requires $\alpha=\mathrm{int}\to\beta$.

**Table of contents**

- [Type unification](type-unification.md)

## ↑ Ancestors (4)

1. [Type system](type-system.md)
2. [Programming language](programming-language.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Algorithm W](algorithm-w.md)
- [Hindley-Milner type system](hindley-milner-type-system.md)
- [Simple type](simple-type.md)
- [Type inference](type-inference.md)
- [Type system](type-system.md)
