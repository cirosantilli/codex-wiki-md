<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The runtime [precondition](../../../../../precondition.md) check rules out negative dimensions:
```
def makeZeroVector(size: Int): Node = {
  require(size >= 0)
  val h = new Node(0.0, size)
  h.prev = h
  h.next = h
  h
}
```
Both links point to the fresh [list header](../../../../../list-header.md), so all reciprocal-link conditions hold and there are no ordinary entries to violate ordering or nonzero-value requirements. The [abstraction function](../../../../../abstraction-function.md) therefore yields **the zero [vector](../../../../../vector.md) of dimension `size`**. Construction uses [constant time](../../../../../constant-time.md) and [constant space](../../../../../constant-space.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
