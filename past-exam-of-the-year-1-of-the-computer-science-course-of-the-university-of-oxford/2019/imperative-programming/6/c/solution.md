<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The plus marks a [covariant type parameter](../../../../../covariant-type-parameter.md): **if $S<:T$, then `Iterator[S] <: Iterator[T]`**. An [iterator](../../../../../iterator.md) producing a subtype's values can be used where an [iterator](../../../../../iterator.md) of the supertype is required. For example, a [string](../../../../../string.md) [iterator](../../../../../iterator.md) can be viewed as an [iterator](../../../../../iterator.md) of `AnyRef`, because [strings](../../../../../string.md) are reference values. The direction is appropriate for a producer: calling `next()` gives a value valid at the wider type. It would not be safe to expose an ordinary insertion method accepting arbitrary wider-type values into a subtype-only collection. This is a [subtyping](../../../../../subtyping.md) relationship, not a request to transform each produced value.[Conformance of parameterized types with covariant parameters](../../../../../scala-2-12-types-specification.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
