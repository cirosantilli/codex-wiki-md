<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

An already-zero entry needs no new [linked list node](../../../../../linked-list-node.md):
```
def zeroElement(vector: Node, index: Int): Unit = {
  require(vector != null)
  require(0 <= index && index < vector.index)
  var p = vector.next
  while ((p ne vector) && p.index < index) p = p.next
  if ((p ne vector) && p.index == index) {
    val left = p.prev
    val right = p.next
    left.next = right
    right.prev = left
  }
}
```
The full input [representation invariant](../../../../../representation-invariant.md) is a [precondition](../../../../../precondition.md). The search has the same [loop invariant](../../../../../loop-invariant.md) and [loop variant](../../../../../loop-variant.md) as in part (d). At exit, either `p` is the only stored entry with that index or none exists. In the first case, bypassing it in both directions removes exactly that coordinate and preserves the order of all remaining entries. This also works when its two neighbors are the same [list header](../../../../../list-header.md), leaving a self-linked empty structure. The header itself is never removed. **The requested coordinate is zero and all others are unchanged**, in $O(k+1)$ [time complexity](../../../../../time-complexity.md).

## ↑ Ancestors (12)

1. [E](../e.md)
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
