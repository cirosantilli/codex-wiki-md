# Generic method

↑ **Parent:** [Parametric polymorphism](parametric-polymorphism.md)

An [object method](object-method.md) with its own [type parameters](type-parameter.md), instantiated or inferred at each call. In [Scala](scala.md), `def identity[T](x: T): T = x` is a generic method. A method `def accept(x: T)` inside `class Box[T]` instead uses a class type parameter fixed by the receiver's [type argument](type-argument.md); it is not itself a generic method with a separately chosen `T` on every call. This distinction matters in [method overloading](method-overloading.md).

## ↑ Ancestors (5)

1. [Parametric polymorphism](parametric-polymorphism.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/5/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming/6/c/solution.md)
