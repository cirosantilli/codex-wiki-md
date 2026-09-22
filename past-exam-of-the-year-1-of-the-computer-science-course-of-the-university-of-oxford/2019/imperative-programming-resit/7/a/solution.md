<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Programming language polymorphism](../../../../../programming-language-polymorphism.md) lets one expression or operation work with values of different types or concrete representations. In [object-oriented programming](../../../../../object-oriented-programming.md), [subtype polymorphism](../../../../../subtype-polymorphism.md) lets a reference of an interface or superclass type designate instances of different implementing [software classes](../../../../../class-programming.md). A call through that reference uses [dynamic dispatch](../../../../../dynamic-dispatch.md) to select the receiver's overriding [object method](../../../../../object-method.md). For example, a routine taking `Book` can invoke `recall` on a linked-list or an array-based implementation while depending only on the common abstract contract.

[Parametric polymorphism](../../../../../parametric-polymorphism.md) is another form: the type parameter in `FiniteDist[T]` lets the same interface describe distributions over [Booleans](../../../../../boolean-data-type.md), [integers](../../../../../integer-split.md) or characters. A generic method introduces a further type parameter when its output type differs. [Method overloading](../../../../../method-overloading.md), in contrast, supplies several statically selected signatures with one name; it should not be confused with receiver-dependent [dynamic dispatch](../../../../../dynamic-dispatch.md). Correct substitutability also requires implementations to respect the common behavioral contract, not merely to share method names.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
