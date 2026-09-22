<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Immutable Scala **`List[+A]` is covariant**: if `Juice` is a subtype of `Drink`, a list of juices can be used as a list of drinks. Scala **`Array[A]` is invariant** because it permits both reading and writing elements.

If an array of juices could be treated as an array of drinks, writing a beer through that widened reference would violate the original juice-array contract. This illustrates [covariant type parameter](../../../../../covariant-type-parameter.md) versus [generic type invariance](../../../../../generic-type-invariance.md); immutability permits the first relationship for lists.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
