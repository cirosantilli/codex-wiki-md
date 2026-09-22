<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep private references `first` and `last`, both initially `null`. A nonempty representation is a finite acyclic chain from `first` through `next` to `last`. Its [representation invariant](../../../../../representation-invariant.md) requires `first.prev == null`, `last.next == null`, and [reciprocal](../../../../../multiplicative-inverse.md) links between every adjacent pair. The nodes reached by following `prev` from `last` are exactly the same nodes in reverse order. No internal node reference is exposed to clients.

The [abstraction function](../../../../../abstraction-function.md) reads the `datum` values along the forward chain, giving the abstract [sequence](../../../../../sequence.md) from left to right. **The empty representation has both endpoint references null**; the [invariant](../../../../../invariant-mathematics.md) requires that either both are null or both are nonnull. A single node has both links null. Updating both endpoint references when removing that last node is therefore essential.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
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
