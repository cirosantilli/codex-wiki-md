<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Follow the next reference for the desired level, stopping at the tail. This returns the genuine nodes in their [linked list](../../../../../linked-list.md) order, excluding both [sentinel nodes](../../../../../sentinel-node.md).
```
def nodesAt(level: Int): List[Node] = {
  require(0 <= level && level < NumLevels)
  val out = scala.collection.mutable.ListBuffer.empty[Node]
  var n = head.nexts(level)
  while (n ne tail) {
    out += n
    n = n.nexts(level)
  }
  out.toList
}
```
Write $L_h$ for the resulting [sequence](../../../../../sequence.md) of nodes at level $h$. The [abstraction function](../../../../../abstraction-function.md) is

$$
\boxed{\alpha=\mathrm{map}(\mathrm{datum},L_0).}
$$

It preserves repetitions, because distinct nodes may carry equal values. A suitable [representation invariant](../../../../../representation-invariant.md) requires the following:

- `head` and `tail` are distinct [sentinel nodes](../../../../../sentinel-node.md) with the specified extreme values; every node has a `nexts` [array](../../../../../array-data-structure.md) of length `NumLevels`.
- For each level, following references from `head` gives a finite acyclic chain ending at `tail`, then `null`; the data along that chain are nondecreasing. Genuine values lie strictly between the [sentinel values](../../../../../sentinel-value.md).
- Each $L_{h+1}$ is a subsequence of $L_h$ **by node identity**, so the relative order of equal-valued nodes agrees across levels. Every genuine node occurs in $L_0$ and on a contiguous initial collection of levels.
- A genuine node absent from a level has `null` in that level's slot. Tail slots are all `null`; every other slot on a chain points to the next member of that chain.

These structural requirements make the traversal terminate and make descending through levels valid. A probabilistic height distribution is a performance policy, rather than a condition needed for the [abstraction function](../../../../../abstraction-function.md) to describe an ordered [sequence](../../../../../sequence.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
