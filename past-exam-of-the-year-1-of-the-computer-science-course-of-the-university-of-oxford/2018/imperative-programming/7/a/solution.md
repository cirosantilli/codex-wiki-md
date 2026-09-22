<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Programming language polymorphism](../../../../../programming-language-polymorphism.md) means that one interface or program definition can be used with values of multiple types. In [object-oriented programming](../../../../../object-oriented-programming.md), [subtype polymorphism](../../../../../subtype-polymorphism.md) allows references with a common [static type](../../../../../static-type.md) to denote instances of different concrete subclasses or implementers of a [trait](../../../../../trait.md). An [object method](../../../../../object-method.md) call uses [dynamic dispatch](../../../../../dynamic-dispatch.md) to select the overriding implementation belonging to the receiver's [runtime type](../../../../../runtime-type.md). For example, different implementations of a playlist interface can respond to the same `insert` call without the client testing their concrete classes.

[Parametric polymorphism](../../../../../parametric-polymorphism.md) uses [type parameters](../../../../../type-parameter.md), as in `Sequence[A]`, so the same definition works uniformly for songs, [integers](../../../../../integer-split.md), or other elements. [Ad hoc polymorphism](../../../../../ad-hoc-polymorphism.md) includes [method overloading](../../../../../method-overloading.md), where different parameter signatures share a name and the [static types](../../../../../static-type.md) determine overload selection. These mechanisms are distinct: selecting an overloaded signature is not the same step as dispatching an override of that selected signature. [Class inheritance](../../../../../class-inheritance.md) can supply implementations, but the reusable interface and legal [subtyping](../../../../../subtyping.md) relationship determine what a polymorphic client may do.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
