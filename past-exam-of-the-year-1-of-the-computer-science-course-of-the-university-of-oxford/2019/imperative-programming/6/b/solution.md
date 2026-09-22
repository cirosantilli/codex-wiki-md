<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The essential abstract methods are:
```
def hasNext: Boolean
def next(): T
```
`hasNext` reports whether another result is available. `next()` returns that result and advances; if exhausted, it throws `NoSuchElementException`. The other ordinary [iterator](../../../../../iterator.md) operations are implemented using these primitives. An availability check must not silently discard a result visible to the client, although an adapter may need to fetch and cache underlying values in order to decide availability.[[Iterator](../../../../../iterator.md) abstract members hasNext and next; exhaustion contract](../../../../../scala-2-12-iterator-api-documentation.md)

## ↑ Ancestors (12)

1. [B](../b.md)
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
