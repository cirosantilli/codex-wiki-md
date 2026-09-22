<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [iterator pattern](../../../../../iterator-pattern.md) when clients need **sequential access to a collection's elements without depending on its internal representation**. A collection supplies a traversal object with operations such as `hasNext` and `next`; the client uses the same traversal interface whether the collection is an [array](../../../../../array-data-structure.md), [linked list](../../../../../linked-list.md), or another [data structure](../../../../../data-structure-split.md).

The [iterator](../../../../../iterator.md) keeps the traversal state separate from both the collection and client, so several independent traversals can coexist and the representation can change without rewriting traversal logic. It can also support incremental or [lazy evaluation](../../../../../lazy-evaluation.md) of elements. Exhaustion must have defined behavior, and a mutable collection must define how updates during traversal are handled. The pattern does not by itself promise that arbitrary concurrent modifications are safe.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
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
