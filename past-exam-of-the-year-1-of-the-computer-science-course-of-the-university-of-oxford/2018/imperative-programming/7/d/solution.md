<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [covariant type parameter](../../../../../covariant-type-parameter.md) preserves [subtyping](../../../../../subtyping.md): **if $A<:B$, then `PartialFn[T,A] <: PartialFn[T,B]`** when its second parameter is covariant. In [Scala](../../../../../scala.md) the class annotation is `+U`. A mapping that produces a narrower output can be used where a broader output is expected. Covariance describes a type relationship; it does not convert stored values or make mutation through a widened reference safe.[Relations between types: conformance of parameterized types and variance](../../../../../scala-2-12-types-specification.md)

## ↑ Ancestors (12)

1. [D](../d.md)
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
