<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use [short-circuit evaluation](../../../../../short-circuit-evaluation.md) so that even an availability test of the second [iterator](../../../../../iterator.md) is delayed until the first is exhausted:
```
class ConcatIterator[T](first: Iterator[T], second: Iterator[T])
    extends Iterator[T] {
  def hasNext: Boolean = first.hasNext || second.hasNext

  def next(): T = {
    if (first.hasNext) first.next()
    else if (second.hasNext) second.next()
    else throw new java.util.NoSuchElementException("empty concatenation")
  }
}
```
Each successful call returns from the first producer while it has entries, then from the second. There is no constructor-time request or element prefetch. This implements concatenation of the producers' remaining [sequences](../../../../../sequence.md), subject to their ordinary [iterator](../../../../../iterator.md) contracts.

## ↑ Ancestors (12)

1. [E](../e.md)
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
