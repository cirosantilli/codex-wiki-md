<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**[Method overloading](../../../../../method-overloading.md)** gives one name several parameter signatures, such as `show(A)` and `show(B)`. The [compiler](../../../../../compiler.md) chooses an applicable signature using the receiver's [static type](../../../../../static-type.md) and the argument expressions' [static types](../../../../../static-type.md), preferring a uniquely more specific applicable alternative. An argument whose type is a [subtype](../../../../../subtyping.md) of the parameter type is acceptable; ambiguous or inapplicable alternatives cause a compile-time error. The [runtime type](../../../../../runtime-type.md) of an argument does not start a second overload search.

**[Method overriding](../../../../../method-overriding.md)** replaces an inherited implementation of the same method signature. After overload selection, ordinary instance calls use [dynamic dispatch](../../../../../dynamic-dispatch.md) on the receiver's [runtime type](../../../../../runtime-type.md) to select the most-derived implementation of that signature. A concrete inherited method requires the `override` keyword in Scala; a `super` call invokes the corresponding superclass implementation instead of redispatching to the overriding body. In a trait stack, `super` follows the class's linearization.[Overloading resolution: applicable alternatives and most-specific selection](../../../../../scala-2-13-expressions-specification.md)[Member lookup, overriding and override modifier](../../../../../scala-2-13-classes-and-objects-specification.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
