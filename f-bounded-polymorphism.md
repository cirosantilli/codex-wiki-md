# F-bounded polymorphism

↑ **Parent:** [Upper type bound](upper-type-bound.md)

A [type parameter](type-parameter.md) can be bounded using a type expression containing that same parameter. In [Scala](scala.md), `[T <: Ordered[T]]` requires each admissible `T` to provide comparison with another `T`. This gives a generic minimum scan access to `x < y` for two elements of type `T`. An arbitrary unrelated upper bound would not establish the needed argument type.

## ↑ Ancestors (6)

1. [Upper type bound](upper-type-bound.md)
2. [Subtyping](subtyping.md)
3. [Type system](type-system.md)
4. [Programming language](programming-language-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/8/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/8/d/solution.md)
