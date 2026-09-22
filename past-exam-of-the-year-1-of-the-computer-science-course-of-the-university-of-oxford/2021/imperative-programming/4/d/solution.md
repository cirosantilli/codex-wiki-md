<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Check that at least one real node exists, then compose the two helpers:

```
def deleteMin(): Int = {
  require(bagHeader.next != null, "bag is empty")
  val smallest = findMin(bagHeader.next)
  val answer = smallest.datum
  delete(smallest)
  answer
}
```

The [precondition](../../../../../precondition.md) check makes `findMin` applicable. Its result belongs to the real-node [sequence](../../../../../sequence.md), satisfying `delete`'s [precondition](../../../../../precondition.md). Consequently **one minimum value is returned and exactly one occurrence is removed**; duplicates remain as distinct nodes. Saving the datum before deletion also separates the return value from subsequent link mutation. Two linear traversals still give $O(m)$ time for a [multiset](../../../../../multiset.md) containing $m$ nodes, with constant auxiliary space.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
