<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [iterator concatenation](../../../../../iterator-concatenation.md) and short-circuit the second availability test while the first [iterator](../../../../../iterator.md) still has results:
```
class ConcatIterator[T](first: Iterator[T], second: Iterator[T])
    extends Iterator[T] {
  def hasNext: Boolean = first.hasNext || second.hasNext

  def next(): T = {
    if (first.hasNext) first.next()
    else second.next()
  }
}
```
The abstract remaining [sequence](../../../../../sequence.md) is the remaining [sequence](../../../../../sequence.md) of `first` followed by that of `second`. Each `next()` consumes the head of precisely this [sequence](../../../../../sequence.md). When both are exhausted, delegation to `second.next()` raises the required exception. **Construction consumes no elements**, and `hasNext` never calls either underlying `next()`. As usual, clients should not separately consume these [iterators](../../../../../iterator.md) while relying on the adapter's traversal. Sharing one underlying [iterator](../../../../../iterator.md) between both arguments also shares its state; it does not duplicate its elements.

## ↑ Ancestors (12)

1. [D](../d.md)
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
