<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume `vector` is a well-formed header satisfying the sparse-vector [representation invariant](../../../../../representation-invariant.md); checking that whole invariant on each operation would require traversing the list. Check the requested bounds and value, then find the first stored coordinate at or after the target.

```
def setElement(vector: Node, value: Double, index: Int): Unit = {
  require(vector != null)
  require(0 <= index && index < vector.index)
  require(value != 0.0 && !value.isNaN && !value.isInfinity)
  var p = vector.next
  while ((p ne vector) && p.index < index) p = p.next
  if ((p ne vector) && p.index == index) p.value = value
  else {
    val fresh = new Node(value, index, p.prev, p)
    p.prev.next = fresh
    p.prev = fresh
  }
}
```

The scan excludes all smaller stored indices. An existing coordinate is updated without duplicating it; otherwise the new node is spliced immediately before `p`, with both directions repaired. The header also serves as the insertion boundary after the final data node. Strict index order and nonzero storage are preserved. The cost is **$O(k)$ search and $O(1)$ pointer work**, where $k$ is the number of stored entries.

## ↑ Ancestors (12)

1. [D](../d.md)
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
