# Covariance failure for a mutable collection

↑ **Parent:** [Covariant type parameter](covariant-type-parameter.md)

Suppose a mutable collection of narrow-type values could be viewed as a mutable collection of a wider type. Inserting a wider-only value through that alias would make a subsequent narrow-type read invalid. For example, hypothetical covariance would let one insert a [string](string.md) through an `Any`-typed alias of an integer multiset. [Generic type invariance](generic-type-invariance.md) prevents that substitution; making a parameter covariant does not authorize an unsound consuming method.

## ↑ Ancestors (6)

1. [Covariant type parameter](covariant-type-parameter.md)
2. [Parametric polymorphism](parametric-polymorphism.md)
3. [Type system](type-system.md)
4. [Programming language](programming-language-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/8/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/8/b/solution.md)
