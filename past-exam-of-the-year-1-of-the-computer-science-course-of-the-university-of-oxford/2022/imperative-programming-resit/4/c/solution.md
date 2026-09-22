<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Permit any nonnegative dimension, including the empty vector:

```
def makeZeroVector(size: Int): Node = {
  require(size >= 0, "negative vector length")
  val head = new Node(0.0, size, null, null)
  head.prev = head
  head.next = head
  head
}
```

This establishes the circular-link [representation invariant](../../../../../representation-invariant.md) in $O(1)$ time and uses one header regardless of the number of implicit zeros. For the nonzero dimension mentioned in part (b), simply use `size > 0` at that call site.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
