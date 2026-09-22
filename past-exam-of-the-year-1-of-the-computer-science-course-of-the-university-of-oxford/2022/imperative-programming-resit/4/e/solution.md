<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

An absent coordinate already has value zero. If found, unlink its node in both directions:

```
def zeroElement(vector: Node, index: Int): Unit = {
  require(vector != null)
  require(0 <= index && index < vector.index)
  var p = vector.next
  while ((p ne vector) && p.index < index) p = p.next
  if ((p ne vector) && p.index == index) {
    p.prev.next = p.next
    p.next.prev = p.prev
  }
}
```

Identity comparison with the header prevents treating its dimension field as a data index. The splice preserves reciprocal links even when removing the only data node: the two header links then point to the header again. All other coordinates are unchanged, and an absent coordinate causes no mutation. **The [running time](../../../../../running-time.md) is $O(k)$**, with constant work after the node is located.

## ↑ Ancestors (12)

1. [E](../e.md)
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
