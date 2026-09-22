<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**[Programming language polymorphism](../../../../../programming-language-polymorphism.md) lets a common interface or operation apply to values of more than one type.** In [subtype polymorphism](../../../../../subtype-polymorphism.md), a variable typed by a base class or trait can refer to instances of different implementing classes. A method call is checked through that common interface, then [dynamic dispatch](../../../../../dynamic-dispatch.md) selects the receiver's overriding implementation. For example, a consumer using `Iterator[Int]` can accept either a filtering [iterator](../../../../../iterator.md) or a concatenating [iterator](../../../../../iterator.md) without knowing its concrete class.

Inheritance can establish a subtype relationship, while [method overriding](../../../../../method-overriding.md) provides distinct implementations of a shared method signature. The classes must still honour the common behavioural contract; sharing a name alone does not establish substitutability. [Parametric polymorphism](../../../../../parametric-polymorphism.md) is different: the type parameter in `Iterator[T]` or `FiniteDist[T]` lets a definition work uniformly over element types. [Method overloading](../../../../../method-overloading.md) is a further form of [software polymorphism](../../../../../programming-language-polymorphism.md) in which the compiler selects a signature using the static argument types; it should not be confused with runtime receiver dispatch.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
