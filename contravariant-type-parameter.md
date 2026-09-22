# Contravariant type parameter

↑ **Parent:** [Parametric polymorphism](parametric-polymorphism.md)

A parameter position for which $S<:T$ implies $F[T]<:F[S]$. In [Scala](scala.md), it is annotated `-`. A consumer capable of accepting every broad-type value can safely serve a context that supplies only narrower values. Returning a value of that parameter type would generally break this guarantee.

## ↑ Ancestors (5)

1. [Parametric polymorphism](parametric-polymorphism.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/8/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/8/a/solution.md)
- [Type variance](type-variance.md)
