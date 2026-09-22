<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Two mechanisms are **[subtype polymorphism](../../../../../subtype-polymorphism.md) and [parametric polymorphism](../../../../../parametric-polymorphism.md)**.

With [subtype polymorphism](../../../../../subtype-polymorphism.md), a [trait](../../../../../trait.md) or [abstract class](../../../../../abstract-class.md) declares an operation and concrete subclasses implement or override it. A `Player` reference holding a `House` object invokes `House.play` through [dynamic dispatch](../../../../../dynamic-dispatch.md). The client is written against the common contract.

With [parametric polymorphism](../../../../../parametric-polymorphism.md), a [software class](../../../../../class-programming.md) or [generic method](../../../../../generic-method.md) has a [type parameter](../../../../../type-parameter.md), such as `List[T]` or `def identity[T](x: T): T = x`. The same definition works for many supplied [type arguments](../../../../../type-argument.md), with static relationships between input and output types. [Method overloading](../../../../../method-overloading.md) is another mechanism, usually called [ad hoc polymorphism](../../../../../ad-hoc-polymorphism.md): alternatives share a name but are selected from their parameter signatures at compile time.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
