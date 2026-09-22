<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes in special cases; an ordinary finite [iterator](../../../../../iterator.md) that progresses through its input needs changing consumption state.** For a genuine immutable [counterexample](../../../../../counterexample.md), an [iterator](../../../../../iterator.md) over an infinite constant [sequence](../../../../../sequence.md) needs no changing fields:
```
final class Ones extends Iterator[Int] {
  def hasNext: Boolean = true
  def next(): Int = 1
}
```
Removing the first entry of that [sequence](../../../../../sequence.md) leaves the same [sequence](../../../../../sequence.md), so this satisfies the [iterator](../../../../../iterator.md) behaviour without changing object state. A permanently empty [iterator](../../../../../iterator.md) is another example.

For a normal finite nonempty traversal, however, repeated `next()` calls must eventually change the returned entry or availability, so the implementation needs mutable cursor state somewhere. Declaring only `val` fields is not a proof of deep immutability: those fields can refer to another mutable [iterator](../../../../../iterator.md), an [array](../../../../../array-data-structure.md), or a stateful closure. The standard API's description of [iterators](../../../../../iterator.md) as mutable captures the usual consuming case, rather than enforcing a mutable field in every possible implementation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
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
