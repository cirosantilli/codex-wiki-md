# Simple type

↑ **Parent:** [Type system](type-system.md)

In the examples here, a [simple type](simple-type.md) is a finite expression built from the base types `int` and `bool` using [function types](function-type.md):

$$
\tau::=\mathrm{int}\mid\mathrm{bool}\mid(\tau\to\tau).
$$

For example, $\mathrm{int}\to\mathrm{bool}$ describes a function accepting an [integer](integer-split.md) and producing a Boolean value. During [type inference](type-inference.md), the grammar is extended with [type variables](type-variable.md) such as $\alpha$ for types not yet determined. A [type scheme](type-scheme.md) additionally binds such [type variables](type-variable.md); it is distinct from the individual [simple type](simple-type.md) used at one call.

## ↑ Ancestors (4)

1. [Type system](type-system.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Function type](function-type.md)
- [Lambda Calculus and Types examination paper of the University of Oxford (2015)](lambda-calculus-and-types-examination-paper-of-the-university-of-oxford-2015.md)
- [Occurs check](occurs-check.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/lambda-calculus-and-types/2/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/lambda-calculus-and-types/2/d/solution.md)
- [Recursive type](recursive-type.md)
- [Simple type](simple-type.md)
- [Type unification](type-unification.md)
- [Universal typing axiom](universal-typing-axiom.md)
