<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The expression constructs a valid [iterator](../../../../../iterator.md) object; it does not itself return the concatenated numeric or character values. The element types have a common supertype `AnyVal`, and covariance lets `Iterator[Int]` and `Iterator[Char]` serve as the two inputs to `ConcatIterator[AnyVal]`. In the ordinary Scala 2 typing of this expression, the common element type is `AnyVal`. One can make the intended widening explicit:
```
new ConcatIterator[AnyVal](
  List(1, 2, 3).iterator,
  List('a', 'b', 'c').iterator
)
```
**Successive calls return `1, 2, 3, 'a', 'b', 'c'`, then exhaustion.** Characters remain characters: viewing an existing [iterator](../../../../../iterator.md) at a wider type does not convert its contents to [integer](../../../../../integer-split.md) character codes. No `next()` is invoked merely by constructing this adapter. The common-type argument uses [subtype polymorphism](../../../../../subtype-polymorphism.md) and [covariant type parameters](../../../../../covariant-type-parameter.md), rather than requiring the two concrete input types to be equal.

## ↑ Ancestors (12)

1. [E](../e.md)
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
