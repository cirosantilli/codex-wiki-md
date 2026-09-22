<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [iterator pattern](../../../../../iterator-pattern.md) separates traversal state from the aggregate being traversed. A client asks whether another entry exists, then requests that entry, without knowing whether storage is an [array](../../../../../array-data-structure.md), a [linked list](../../../../../linked-list.md) or another [data structure](../../../../../data-structure-split.md). Distinct [iterators](../../../../../iterator.md) have independent positions in a traversal.

In [Java](../../../../../java-programming-language.md), declare `DataList implements Iterable<Point>` and provide `public Iterator<Point> iterator()`. The returned [iterator](../../../../../iterator.md) implements `hasNext()` and `next()`; exhausted `next()` throws `NoSuchElementException`. This also permits an enhanced `for (Point p : data)` loop.[Iterable.iterator(), enhanced for support, and Iterator.next() exhaustion contract](../../../../../java-8-iteration-api-documentation.md)

Returning `points.iterator()` directly would permit removal through that [iterator](../../../../../iterator.md) and expose mutable stored `Point` instances. Part (e) instead returns an unmodifiable [iterator snapshot](../../../../../iterator-snapshot.md) containing fresh `Point` copies. That choice gives stable traversals and prevents [representation exposure](../../../../../representation-exposure.md), with the tradeoff that a traversal does not see subsequent insertions. Thus

$$
\boxed{\texttt{Iterable<Point>}\ \text{creates independent}\ \texttt{Iterator<Point>}\ \text{traversals}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Object oriented programming](../../../object-oriented-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
