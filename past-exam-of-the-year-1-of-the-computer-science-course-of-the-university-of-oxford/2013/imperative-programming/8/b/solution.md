<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If the mutable [set](../../../../../set-split.md) were allowed a [covariant type parameter](../../../../../covariant-type-parameter.md), both variables below could refer to the same mutable object:
```
val s1: Set[Int] = new Set[Int](List())
val s2: Set[Any] = s1             // hypothetically permitted
s2.add("not an integer")
val n: Int = s1.delete()         // cannot return an Int
```
The broad view accepts any value, including a [string](../../../../../string.md). The narrow view still promises that deletion returns an `Int`, yet the sole stored value is that [string](../../../../../string.md). This violates [type safety](../../../../../type-safety.md):

$$
\boxed{\text{A mutable collection that both accepts and returns }T\text{ cannot be covariant in }T.}
$$

This is [covariance failure for a mutable collection](../../../../../covariance-failure-for-a-mutable-collection.md). The input occurrence in `add(x: T)` conflicts with the positive occurrence in the result of `delete`. Keeping a [generic type invariance](../../../../../generic-type-invariance.md) restriction prevents the unsafe aliasing. The example uses an initially empty [set](../../../../../set-split.md) so that the problematic deletion result is forced.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
